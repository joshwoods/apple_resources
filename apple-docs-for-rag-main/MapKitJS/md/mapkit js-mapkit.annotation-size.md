

- MapKit JS
- mapkit.Annotation
-  size 

Instance Property

# size

The desired dimensions of the annotation, in CSS pixels.

MapKit JS 5.0+

``` source
attribute Object size;
```

## Discussion

If supplied, indicates the desired size of the annotation in CSS pixels. The value must be an object with `width` and `height` number properties:

```
{
    size: { width: 32, height: 39 }
}
```

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

visible

A Boolean value that determines whether the annotation is visible or hidden.

