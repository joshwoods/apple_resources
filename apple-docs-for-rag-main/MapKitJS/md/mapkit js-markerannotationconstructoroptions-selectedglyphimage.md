

- MapKit JS
- MarkerAnnotationConstructorOptions
-  selectedGlyphImage 

Instance Property

# selectedGlyphImage

The image to display in the balloon when the user selects the marker.

MapKit JS 5.0+

``` source
attribute Object selectedGlyphImage;
```

## Discussion

Provide glyph images as object literals containing absolute or relative URLs to standard, 2x, and 3x Retina display assets. The framework requires at least one image. MapKit JS displays the selected glyph image in the balloon when the marker is in the selected state. If you specify an image for this property, also specify an image in the glyphImage property.

Set the size of the selected glyph image to 40 x 40 pixels. MapKit JS scales glyph images to fit in the balloon. If you don’t set selectedGlyphImage, the framework uses glyphImage when the user selects the marker. The default image is a pin.

## See Also

### Setting marker annotation properties

color

The background color of the balloon.

glyphColor

The fill color of the glyph.

glyphText

The text to display in the marker balloon.

glyphImage

The image to display in the marker balloon.

subtitleVisibility

A value that determines the behavior of the subtitle’s visibility.

titleVisibility

A value that determines the behavior of the title’s visibility.

