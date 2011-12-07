Resizable
===============

The jQuery resizable plugin resizes images making them full-screen images. There are plenty of plugins that do this for background images, but this works on img tags, divs, whatever.

Useage
----------

Use a jQuery selector to apply the behavior to the objects you want to make full-screen. For example, you could add a class name of "gallery-photo" to your images. Use the following to apply the behavior to your images:

$('gallery-photo').resizable();

There are a few options you can pass as an object to the resizable function:
* centeredY: {true|false} automatically centers the image vertically (default is true)
* centeredX: {true|false} automatically centers the image horizontally. (default is true)* addWidthHeightAttributes: {true|false} adds html attributes for width & height to img tags (default is true. ignored for objects that are not img tags)* maxWidth: set a maximum width for the object (useful if you don't want images to overscale)
* maxHeight: set a maximum height for the object (useful if you don't want images to overscale)

The function call should be wrapped in $(document).ready() to make sure that the image tags are available in the DOM when called.

Useage Example
----------------------

The complete useage example is as follows:

$(doument).ready(function() {
  $('.gallery-photo').resizable({centeredX:false,centeredY:false});
});

