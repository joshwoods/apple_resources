

- MapKit JS
- MarkerAnnotationConstructorOptions
-  glyphImage 

Instance Property

# glyphImage

The image to display in the marker balloon.

MapKit JS 5.0+

``` source
attribute Object glyphImage;
```

## Mentioned in 

MapKit JS 5

## Discussion

The glyph image values need to be object literals containing absolute or relative URLs to standard, 2x, and 3x Retina display assets. The framework requires at least one image at 20 x 20 pixels.

MapKit JS uses the default glyph image of a pin if you set glyphImage to `null`, `undefined`, or “” (an empty string). If you specify both a glyphImage and glyphText, the framework ignores the glyph image and displays the glyph text.

## See Also

### Setting marker annotation properties

color

The background color of the balloon.

glyphColor

The fill color of the glyph.

glyphText

The text to display in the marker balloon.

selectedGlyphImage

The image to display in the balloon when the user selects the marker.

subtitleVisibility

A value that determines the behavior of the subtitle’s visibility.

titleVisibility

A value that determines the behavior of the title’s visibility.

