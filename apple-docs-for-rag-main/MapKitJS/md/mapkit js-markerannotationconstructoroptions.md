

- MapKit JS
-  MarkerAnnotationConstructorOptions 

Structure

# MarkerAnnotationConstructorOptions

An object containing the options that create a marker annotation.

MapKit JS 5.0+

``` source
dictionary MarkerAnnotationConstructorOptions {
 string titleVisibility;
 string subtitleVisibility;
 string color;
 string glyphColor;
 string glyphText;
 Object glyphImage;
 Object selectedGlyphImage;
};
```

## Topics

### Setting marker annotation properties

color

The background color of the balloon.

glyphColor

The fill color of the glyph.

glyphText

The text to display in the marker balloon.

glyphImage

The image to display in the marker balloon.

selectedGlyphImage

The image to display in the balloon when the user selects the marker.

subtitleVisibility

A value that determines the behavior of the subtitle’s visibility.

titleVisibility

A value that determines the behavior of the title’s visibility.

## See Also

### Creating a marker annotation

mapkit.MarkerAnnotation

Creates a marker annotation at the coordinate location with provided options.

