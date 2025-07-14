

- Foundation
- NSAffineTransform
-  translateX(by:yBy:) 

Instance Method

# translateX(by:yBy:)

Applies the specified translation factors to the receiver’s transformation matrix.

Mac Catalyst 13.0+macOS 10.0+

``` source
func translateX(
    by deltaX: Double,
    yBy deltaY: Double
)
```

## Parameters 

`deltaX`  

The number of units to move along the x axis.

`deltaY`  

The number of units to move along the y axis.

## Discussion

Subsequent transformations cause coordinates to be shifted by `deltaX` units along the x axis and by `deltaY` units along the y axis. Translation factors do not affect `NSSize` values, which specify a differential between points.

## See Also

### Accumulating Transformations

func rotate(byDegrees: Double)

Applies a rotation factor (measured in degrees) to the receiver’s transformation matrix.

func rotate(byRadians: Double)

Applies a rotation factor (measured in radians) to the receiver’s transformation matrix.

func scale(by: Double)

Applies the specified scaling factor along both x and y axes to the receiver’s transformation matrix.

func scaleX(by: Double, yBy: Double)

Applies scaling factors to each axis of the receiver’s transformation matrix.

func append(NSAffineTransform)

Appends the specified matrix to the receiver’s matrix.

func prepend(NSAffineTransform)

Prepends the specified matrix to the receiver’s matrix.

func invert()

Replaces the receiver’s matrix with its inverse matrix.

