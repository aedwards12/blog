---
layout: post
title:  "Margins, Borders, and Padding"
date:   2014-06-06 16:24:54
categories: jekyll update
---

#### Overview
All html block-level elements have five spacing properties: height, width, margin, border, and padding. When using these properties, we are primarily working with < div > tags or another block level element. < div > tags allow you to wrap, style, and position text in your webpage.


### Border
Border properties allow you to specify the style and color of and elements border. ex: 
{% highlight ruby %}
border: 1px solid black;
border-bottom: 2px solid rgba(255,255,200, .7);
{% endhighlight %}
![alt text][border]


### Padding
Padding can be effectively be used to push or limit the content inside a block element. Think of it as putting up a railing before a cliff. Nothing can occupy that space between the railing and cliff. Padding also has 4 properties that can be changed independently top, bottom, left, and right. ex:
{% highlight ruby %}
padding: 10px;
padding: 10px 30px; #same as padding: 10px 30px 10px 30px;
padding-left: 30px;
{% endhighlight %}
![alt text][padding]


### Margin
Margins clear an area around an element outside the border. Margins prevent other element from getting to close. In other words give me "back up, give me space." Margins have 4 properties that can be changed independently top, bottom, left, and right. ex:

{% highlight ruby %}
margin-top: 30px;
margin: 30px 20px;
{% endhighlight %}
![alt text][margin]


[padding]: http://i1372.photobucket.com/albums/ag340/anthonyedwardsjr/ScreenShot2014-05-06at23607AM_zps280c0fb6.png"padding-image"
[margin]: http://i1372.photobucket.com/albums/ag340/anthonyedwardsjr/ScreenShot2014-05-06at23116AM_zpsb0ad8df8.png "margin-image"
[border]: http://i1372.photobucket.com/albums/ag340/anthonyedwardsjr/ScreenShot2014-05-06at24040AM_zps73161d19.png "border-image"

