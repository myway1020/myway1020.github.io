---
layout: default
title: About
permalink: about/
render: dynamic
---

This is a base theme for the Material Bliss Jekyll theme. You can find out more info about customizing your Jekyll theme, as well as basic Jekyll usage documentation at [jekyllrb.com](http://jekyllrb.com/), as well as this themes homepage: [Material Bliss](http://www.github.com/InsidiousMind/material-bliss-jekyll-theme)

You can find the source code for the Jekyll Material Bliss Theme at:
{% include icon-github.html username="InsidiousMind" %} /
[material-bliss](https://github.com/InsidiousMind/material-bliss-jekyll-theme)

You can find the source code for Jekyll at
{% include icon-github.html username="jekyll" %} /
[jekyll](https://github.com/jekyll/jekyll)

Here's a demo of syntax highlighting!

{% highlight zsh %}
demo_mod1_generator() {
  local mod="$1" ice="$2"

  #Content, no hyper-links
  reply=( "Hello World from ${ZUI[YELLOW]}ZUI${ZUI[COLOR_END]}! Module $mod, instance $ice." )

  #Non-selectable lines   Hops to jump with [ and ]   Local anchors
  reply2=( )               reply3=( 1 )                reply4=( )
}
{% endhighlight %}


```python
#!/usr/bin/python3

def something:
  print("Hello World!")

something
```

Even though it's built with React and Jekyll, you can still use liquid tags in you're markdown exactly as you would normally! for example, if you look at the sourcecode for this about page, you will find I use this liquid in this very page
