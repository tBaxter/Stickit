Stickit
=======

###Sticky side nav + sticky header + collapsing header. Keep it all stuck where you want it.

Stickit allows for multiple sticky elements, allows them be combined with a sticky header,
allows for expanding/collapsing header navigation,  and prevents overflow of the sticky element to the
header or footer.

The sticky sidebar functionality is based on stickymojo.js: http://mojotech.github.com/stickymojo/
If that's all you need, then use it. They make a nice product.

If using a collapsing header, you can hide/show content in the header based on body.collapsed. 
When collapsed, the class will exist. When open, it won't.


Initialization:
Pass a class name for the elements you want to be sticky, along with a couple of required variables:

$(window).load(function() {
    $('.sticky').stickit({
    footer:  '#footer',
    header:  '#header'
  });
});

* additional settings:
* - stickHeader: false      (if header should not stick)
* - collapseHeader: false   (no collapsing will be done)
