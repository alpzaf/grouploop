## grouploop.js - A simple jQuery plugin

A jquery plugin that creates a marquee with any group of DOM elements, with a variety of options.

### Setup

Include jQuery and the library in your html:

`<script type="text/javascript" src="dist/grouploop-1.0.0.min.js"></script>`

Create a container with a unique id and group some elements in a wrapper.

```
<div id="grouploop-1">
  <div class="item-wrap">
    <div class="item">Promo 1</div>
    <div class="item">Promo 2</div>
    <div class="item">Promo 3</div>
    <div class="item">Promo 4</div>
    <div class="item">Promo 5</div>
    ...
  </div>
</div>
```

Select your DOM element id with jQuery and call **_.grouploop()_** with or without options.

```
$("#grouploop-1").grouploop({
  velocity: 2,
  forward: false,
  childNode: ".item",
  childWrapper: ".item-wrap",
  pauseOnHover: true,
  complete: function() {
    console.log("init");
}
```