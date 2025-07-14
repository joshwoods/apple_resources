

- MapKit JS
- MarkerAnnotationConstructorOptions
-  titleVisibility 

Instance Property

# titleVisibility

A value that determines the behavior of the title’s visibility.

MapKit JS 5.0+

``` source
attribute string titleVisibility;
```

## Discussion

The title visibility controls the title that renders below the balloon part of the marker. The default value is Adaptive.

For adaptive visibility, the title is always visible in the normal state, by default. When the user selects the marker, the title is visible unless the marker’s selected state requires a callout.

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

selectedGlyphImage

The image to display in the balloon when the user selects the marker.

subtitleVisibility

A value that determines the behavior of the subtitle’s visibility.

