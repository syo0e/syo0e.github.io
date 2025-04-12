---
title: "Call signature와 Generci 타입"
layout: post
---

##Call Signature

타입스크립트의 중요 개념 중 하나인 call signature에 대해서 알아보자. 콜 시그니처란 함수 위에 커서를 올리면 나오는 파라미터와 리턴 타입 정보를 말한다. 콜 시그니처는 함수를 만들기 전에 먼저 다음과 같이 타입을 정할 수 있다.

`type Add = (a: number, b: number) => number`

여기서 Add 타입은 a 숫자값과 b 숫자값을 더한 값을 리턴하기 위한 함수의 타입이다. 이렇게 먼저 타입을 정하면 다음과 같이 함수를 구현할 수 있다.

`const add: Add = (a,b) => a + b`

이렇게 때문에 함수를 구현할 때 파라미터나 리턴값의 타입을 따로 고려하면서 작성할 필요가 없다. 즉, 장점이라 하면 디자인 시에 타입을 결정해야하기 때문에 개발자가 타입을 생각하고 작성할 수 있게 한다. 타입스크립트의 특징은 바로 자바스크립트 형태로 컴파일된다는 것인데 얘는 자바스크립트로 컴파일 되지 않는다.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]: https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
