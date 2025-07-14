

- Foundation
- NSAffineTransform
-  scaleX(by:yBy:) 

Instance Method

# scaleX(by:yBy:)

Applies scaling factors to each axis of the receiver’s transformation matrix.

Mac Catalyst 13.0+macOS 10.0+

``` source
func scaleX(
    by scaleX: Double,
    yBy scaleY: Double
)
```

## Parameters 

`scaleX`  

The scaling factor to apply to the x axis.

`scaleY`  

The scaling factor to apply to the y axis.

## Discussion

After invoking this method, applying the receiver’s matrix modifies the unit length on the x axis by a factor of `scaleX` and the y axis by a factor of `scaleY`, in addition to performing all previous transformations. A value of 1.0 for either axis scales the content on that axis to the same size.

## See Also

### Accumulating Transformations

func rotate(byDegrees: Double)

Applies a rotation factor (measured in degrees) to the receiver’s transformation matrix.

func rotate(byRadians: Double)

Applies a rotation factor (measured in radians) to the receiver’s transformation matrix.

func scale(by: Double)

Applies the specified scaling factor along both x and y axes to the receiver’s transformation matrix.

func translateX(by: Double, yBy: Double)

Applies the specified translation factors to the receiver’s transformation matrix.

func append(NSAffineTransform)

Appends the specified matrix to the receiver’s matrix.

func prepend(NSAffineTransform)

Prepends the specified matrix to the receiver’s matrix.

func invert()

Replaces the receiver’s matrix with its inverse matrix.

