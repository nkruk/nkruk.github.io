---
layout: post
title:  "How to update a Github Pages Jekyll blog after years of inactivity"
date:   2023-08-26 13:43:15 +0100s
categories: 
  jekyll
---

Check out [`this docs page`][testing-jekyll-locally].

It's been two years. You don't even remember how to run this locally, don't you?

{% highlight ruby %}
bundle exec jekyll serve
{% endhighlight %}

Ah, but if you're running a ruby version > 3.1.2 then you're screwed. 
Switch to 3.1.2 (using your beloved `chruby`). At least according to [`this issue comment`][problem-with-jekyll].

[testing-jekyll-locally]: https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll
[problem-with-jekyll]: https://github.com/jekyll/jekyll/issues/9233#issuecomment-1365790440