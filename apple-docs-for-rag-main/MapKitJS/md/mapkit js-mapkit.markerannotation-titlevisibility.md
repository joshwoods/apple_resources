

- MapKit JS
- mapkit.MarkerAnnotation
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

### Setting visibility

subtitleVisibility

A value that determines the behavior of the subtitle’s visibility.

mapkit.FeatureVisibility

Constants indicating the visibility of different adaptive map features.

