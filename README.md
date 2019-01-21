# iCheck Font

Adds font functionality to iCheck.js
Currently this is written in SASS but will port to SCSS, (Stylus?) and Less in the future.

![showcase](https://raw.githubusercontent.com/stevenvg/icheck-font/master/img/showcase1.gif)

### Prerequisites

The things you'll need

- **FontForge** if you want to extend the font source or build a fresh .woff or .\*.
- **Illustrator** for the .AI file, but there are SVG files for your convenience.
- **SASS compiler** Grunt, gulp, etc. If you use the sass file.
- **Original Fronteed/iCheck.js javascript file** its not included in this repo.

## Instructions

Include jquery, the original iCheck javascript and the stylesheet from here.
There are options inside the SASS file, but can be totally stripped to the bare minimum with ease.

in the head
```html
<link rel="stylesheet" link="STYLESHEET_PATH/icheck.css">
```

before the body
```html
<script src="PATH_TO_JQUERY.JS"></script>
<script src="PATH_TO_ICHECK.JS"></script>

//init icheck

<script>
  $(document).ready(function() {
    return $('input').iCheck({
      checkboxClass: 'icheckbox_flat',
      radioClass: 'iradio_flat'
    });
  });
</script>
```

**don't forget to include the font file, it is located in the fonts directory one directory up from the stylesheet directory**

## Demo

[demo](https://stevenvg.github.com/icheck-font)

## Compatibility
As long as the browser supports ``` ::before  ``` in CSS it should all be fine.
Tested in following browsers, both mobile and desktop on windows 10/Android:
* Internet explorer(latest)
* Edge
* Firefox
* Chrome

## Contributing

For contributing, open a new issue. we'll get it sorted.

## Acknowledgments

* [fronteed/icheck](https://github.com/fronteed/icheck) - Original iCheck.js repo.
