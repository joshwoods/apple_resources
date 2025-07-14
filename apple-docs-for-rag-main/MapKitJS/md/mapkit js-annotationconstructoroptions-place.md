

- MapKit JS
- AnnotationConstructorOptions
-  place 

Instance Property

# place

An object that allows a custom annotation to potentially supecede a point of interest at the same map coordinates.

MapKit JS 5.76.76+

``` source
attribute Place place;
```

## Discussion

By using a Place object as an argument to the AnnotationConstructorOptions, you can, depending on the exact coordinates and other rendering computations, supersede an Apple-provided item on the map. This can reduce potential visual clutter of two icons representing the same place on a single map.

You can also use a `Place` as the first argument when creating a mapkit.Annotation, rather than using a mapkit.Coordinate to achieve the same effect.

MapKit JS also supports this capability for the initializer and constructor options for mapkit.ImageAnnotation and mapkit.MarkerAnnotation.

## See Also

### Creating interaction behavior

animates

A Boolean value that determines whether the map animates the annotation.

draggable

A Boolean value that determines whether the user can drag the annotation.

enabled

A Boolean value that determines whether the annotation responds to user interaction.

selected

A Boolean value that determines whether the map displays the annotation in a selected state.

