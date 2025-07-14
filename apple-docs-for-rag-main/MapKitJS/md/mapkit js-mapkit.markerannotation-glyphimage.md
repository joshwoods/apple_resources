

- MapKit JS
- mapkit.MarkerAnnotation
-  glyphImage 

Instance Property

# glyphImage

The image to display in the marker balloon.

MapKit JS 5.0+

``` source
attribute Object|ImageDelegate glyphImage;
```

## Discussion

Glyph image values are object literals that contain absolute or relative URLs to standard, `@2x`, and `@3x` assets. Alternatively, you can set an ImageDelegate, which is an object you use to specify image URLs.

The framework requires at least one image at 20 x 20 pixels. Create glyph images as template images — a monochrome image with opacity, if needed — so that MapKit JS can apply the glyphColor to tint to the image.

If you set glyphImage to `null`, `undefined`, or “” (an empty string), MapKit JS uses the default glyph image of a pin. If you specify both a glyphImage and glyphText, MapKit JS ignores the glyph image, and the framework displays glyph text.

## See Also

### Setting the glyph image and text

glyphText

The text to display in the marker balloon.

selectedGlyphImage

The image to display in the marker balloon when the user selects the marker.

