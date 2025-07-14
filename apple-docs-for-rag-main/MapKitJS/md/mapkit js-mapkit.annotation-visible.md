

- MapKit JS
- mapkit.Annotation
-  visible 

Instance Property

# visible

A Boolean value that determines whether the annotation is visible or hidden.

MapKit JS 5.0+

``` source
attribute boolean visible;
```

## Discussion

Set this property to `false` to temporarily hide an annotation.

If there’s a dense cluster of annotations at low zoom levels, it’s good practice to hide some annotations.

## See Also

### Getting and setting annotation appearance

coordinate

The annotation’s coordinate.

anchorOffset

An offset that changes the annotation’s default anchor point.

appearanceAnimation

A CSS animation that runs when the annotation appears on the map.

displayPriority

A numeric hint that the map uses to prioritize how it displays annotations.

mapkit.Annotation.DisplayPriority

Constant values that provide a hint the map uses to prioritize displaying annotations.

padding

Spacing to add around the annotation when showing items.

size

The desired dimensions of the annotation, in CSS pixels.

