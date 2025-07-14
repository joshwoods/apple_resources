

- MapKit JS
- mapkit.MarkerAnnotation
-  selectedGlyphImage 

Instance Property

# selectedGlyphImage

The image to display in the marker balloon when the user selects the marker.

MapKit JS 5.0+

``` source
attribute Object|ImageDelegate selectedGlyphImage;
```

## Mentioned in 

MapKit JS 5

## Discussion

Glyph image values are object literals that contain absolute or relative URLs to standard, `@2x`, and `@3x` assets. Alternatively, you can set an ImageDelegate, which is an object you use to specify image URLs.

The framework requires at least one image and displays the selected glyph image in the balloon when the marker is in the selected state. If you specify an image for this property, also specify an image in the glyphImage property.

Set the size of the selected glyph image to 40 x 40 pixels. Create glyph images as template images — a monochrome image with opacity, if needed — so that MapKit JS can apply the glyphColor to tint to the image. MapKit JS scales glyph images to fit in the balloon. If you don’t set selectedGlyphImage, the framework uses glyphImage when the user selects the marker. The default image is a pin.

## See Also

### Setting the glyph image and text

glyphText

The text to display in the marker balloon.

glyphImage

The image to display in the marker balloon.

