

- MapKit JS
- mapkit.MarkerAnnotation
-  glyphText 

Instance Property

# glyphText

The text to display in the marker balloon.

MapKit JS 5.0+

``` source
attribute string glyphText;
```

## Mentioned in 

Clustering annotations

## Discussion

This property is the text to display in the balloon instead of displaying a glyph image. The default value is `""` (empty string). There’s a limited amount of space available for displaying glyph text. Specify no more than two or three characters.

If you specify both a glyphImage and glyphText, MapKit JS ignores the glyph image, and displays the glyph text.

## See Also

### Setting the glyph image and text

glyphImage

The image to display in the marker balloon.

selectedGlyphImage

The image to display in the marker balloon when the user selects the marker.

