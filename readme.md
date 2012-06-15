Backbone.touch v0.1
=============================

Created by Raymond Julin [@nervetattoo](http://twitter.com/nervetattoo)

A drop in replacement for Backbone.View that enables fast tap events
on touch devices.

## Usage ##

Backbone.touch is made to work with your existing views.
It replaces the `delegateEvents` method and replaces any *click* event
with the three events *touchstart*, *touchmove* and *touchend* when a touch
device is used. Once the touchend fires your callback is executed without the
300ms delay that the *click* event has.

## Download & Include ##

* [Development](https://raw.github.com/nervetatoo/backbone.touch/blob/master/backbone.touch.js)
* [Production](https://raw.github.com/nervetatoo/backbone.touch/blob/master/dist/backbone.touch.min.js)

Depends on Underscore, Backbone and jQuery.  You can swap out the 
jQuery dependency completely with a custom configuration.

Include in your application *after* jQuery, Underscore, and Backbone have been
included.

``` html
<script src="/js/jquery.js"></script>
<script src="/js/underscore.js"></script>
<script src="/js/backbone.js"></script>

<script src="/js/backbone.touch.js"></script>
```

Note that backbone.touch currently overwrites `Backbone.View` to make its usage
a no-op part from including it.

## Release notes ##

### 0.1 ###

* Initial release. Only tested on iPad
