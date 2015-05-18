jQuery Hover Truncated
======

This is a simple jQuery plugin which truncates a text to single line, clipped
with an ellipsis and displays a tooltip on hover. See demo for more details.

Installation and usage
----------------------

1. Run `bower install jquery-hover-truncated`
2. Copy styles to your stylesheet or just link an external file in your `<head>`:

  `<link rel="stylesheet" type="text/css" href="path/to/jquery.hovertruncated.css">`

3. Then, before your closing `<body>` tag add:

  ```
  <script src="path/to/jquery.min.js"></script>
  <script src="path/to/jquery.hovertruncated.js"></script>
  ```

4. In your JS, initialize a plugin:

  ```
  $(function(){
     $('.truncate').hoverTruncated();
  });
  ```

  Or configure it like the following:

  ```
  $(function(){
    var options = {
      dataAttr:    'plugin-cache',    // data attribute to store an instance, default: 'hover-truncated'
      className:   'tooltip-plain',   // tooltip class name, default: 'hover-truncated'
      tooltipText: 'Hello, World!',     // tooltip text, default: element inner text
      offsetX:     0,                 // tooltip offset-x, default: 10px
      offsetY:     0                  // tooltip offset-y, default: 10px
    };
    $('.truncate').hoverTruncated(options);
  });
  ```

5. Then you can call a plugin method:

```
$(function(){
   $('.truncate').hoverTruncated('hide');                             // hides an element's tooltip
   $('.truncate').hoverTruncated('show');                             // reveals an element's tooltip
   $('.truncate').hoverTruncated('update', 'Goodbye, cruel world!');  // updates an element's tooltip content
   $('.truncate').hoverTruncated('destroy');                          // hides and destroys an element's tooltip
});
```

License
-------

This plugin is released under the MIT license.
