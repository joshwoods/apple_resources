

- MapKit JS
- MarkerAnnotationConstructorOptions
-  subtitleVisibility 

Instance Property

# subtitleVisibility

A value that determines the behavior of the subtitle’s visibility.

MapKit JS 5.0+

``` source
attribute string subtitleVisibility;
```

## Discussion

The subtitle visibility controls the subtitle that renders below the balloon part of the marker. The default value is Adaptive.

For adaptive visibility, the subtitle is always hidden in the normal state, by default. In the selected state, the subtitle follows the same rules as the title.

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

titleVisibility

A value that determines the behavior of the title’s visibility.

