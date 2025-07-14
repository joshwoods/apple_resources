

- Group Activities
- SpatialTemplateElementDirection
-  rotatedBy(\_:) 

Instance Method

# rotatedBy(\_:)

Returns a new direction structure that adds the specified rotation angle to the current direction’s value.

visionOS 2.0+

``` source
func rotatedBy(_ rotationAngle: Angle2D) -> SpatialTemplateElementDirection
```

## Parameters 

`rotationAngle`  

The amount of rotation to apply along the y-axis.

## Return Value

A new direction structure that combines the rotation value of the current structure and the `rotationAngle` value.

