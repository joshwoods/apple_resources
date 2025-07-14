

- MapKit JS
- MarkerAnnotationConstructorOptions
-  glyphText 

Instance Property

# glyphText

The text to display in the marker balloon.

MapKit JS 5.0+

``` source
attribute string glyphText;
```

## Discussion

The text to display in the balloon instead of a glyph image. The default value is `""` (empty string). There’s a limited amount of space available for displaying glyph text. Specify no more than two or three characters.

If you specify both a glyphImage and glyphText, MapKit JS ignores the glyph image and displays the glyph text.

## See Also

### Setting marker annotation properties

color

The background color of the balloon.

glyphColor

The fill color of the glyph.

glyphImage

The image to display in the marker balloon.

selectedGlyphImage

The image to display in the balloon when the user selects the marker.

subtitleVisibility

A value that determines the behavior of the subtitle’s visibility.

titleVisibility

A value that determines the behavior of the title’s visibility.

