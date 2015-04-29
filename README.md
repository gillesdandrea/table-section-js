# table-section-js

table-section-js is a jQuery plugin adding sticky headers and/or sections "à la" iOS for HTML tables.
Twitter Bootstrap is recommended but not mandatory.

See table-section-js in action: http://codepen.io/gillesdandrea/pen/aOzewP


## Usage

First, load table-section-js stylesheet:

```html
<link href="css/table-section.css" rel="stylesheet">
```

Then, load jQuery and table-section-js JavaScript:

```html
<script src="js/jquery.js" type="text/javascript"></script>
<script src="js/table-section.js" type="text/javascript"></script>
```

Now, add css class `ts-table-section` to `table` tags and
`ts-row-section` to `tr` tags to be used as table row sections.

```html
<table class="ts-table-section">
  ...
  <tr class="ts-row-section">
    ...
  </tr>
  <tr>
    ...
  </tr>
  ...
</table>
```

Now, run the script on DOM ready:

```html
<script type="text/javascript">
   jQuery(document).ready(function() {
     $(document).tableSection();
   });
</script>
```

You can specify a vertical offset if necessary. I.e when using bootstrap navbar:

```html
<script type="text/javascript">
   jQuery(document).ready(function() {
     $(document).tableSection({verticalOffset: 40});
   });
</script>
```


## TODO

Unit testing, benching, multiple row section support, better iOS scroll support...


## Credits

Many thanks to Ole Morten Amundsen and Brad Birdsall.
Their respective work https://github.com/oma/table-fixed-header and http://css-tricks.com/persistent-headers/ inspired table-section-js.


## Author

[Gilles d'Andréa](http://about.me/gilles.dandrea) ([@gillesdandrea](http://twitter.com/gillesdandrea))
