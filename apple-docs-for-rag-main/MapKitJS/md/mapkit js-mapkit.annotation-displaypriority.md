

- MapKit JS
- mapkit.Annotation
-  displayPriority 

Instance Property

# displayPriority

A numeric hint that the map uses to prioritize how it displays annotations.

MapKit JS 5.0+

``` source
attribute number displayPriority;
```

## Mentioned in 

MapKit JS 5

## Discussion

Maps use the display priority as a hint to determine whether to display annotations at any given time. By default, the display priority is Required, which indicates the annotation always displays on the map.

Display priority can be any number from `0` to `1000`. There are three preset values:

- Low (`250`)

- High (`750`)

- Required (`1000`)

Maps ignore this value when collisionMode is `None`.

## See Also

### Getting and setting annotation appearance

coordinate

The annotation’s coordinate.

anchorOffset

An offset that changes the annotation’s default anchor point.

appearanceAnimation

A CSS animation that runs when the annotation appears on the map.

mapkit.Annotation.DisplayPriority

Constant values that provide a hint the map uses to prioritize displaying annotations.

padding

Spacing to add around the annotation when showing items.

size

The desired dimensions of the annotation, in CSS pixels.

visible

A Boolean value that determines whether the annotation is visible or hidden.

