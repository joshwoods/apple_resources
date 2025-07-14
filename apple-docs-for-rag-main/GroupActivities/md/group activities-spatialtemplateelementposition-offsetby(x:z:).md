

- Group Activities
- SpatialTemplateElementPosition
-  offsetBy(x:z:) 

Instance Method

# offsetBy(x:z:)

Returns a new position at the specified distance from the origin of the shared coordinate space.

visionOS 2.0+

``` source
func offsetBy(
    x: Double,
    z: Double
) -> SpatialTemplateElementPosition
```

## Parameters 

`x`  

The distance from the current position, in meters, along the x-axis. You can specify positive or negative values to specify new positions on either side of the original position.

`z`  

The distance from the current position, in meters, along the z-axis. You can specify positive or negative values to specify new positions on either side of the original position.

## Return Value

A position structure with the specified offsets from the current position.

## Discussion

Use this method to adjust an existing position by the specified number of meters. The x- and y-axes form a plane that is horizontal to the ground. The following example creates a new position that is four meters from the app’s content along the z-axis:

```
let audienceCenterPoint = SpatialTemplateElementPosition.app.offsetBy(x: 0, z: 4)
```

