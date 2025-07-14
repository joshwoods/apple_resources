

- MapKit JS
- mapkit.MarkerAnnotation
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

### Setting visibility

titleVisibility

A value that determines the behavior of the title’s visibility.

mapkit.FeatureVisibility

Constants indicating the visibility of different adaptive map features.

