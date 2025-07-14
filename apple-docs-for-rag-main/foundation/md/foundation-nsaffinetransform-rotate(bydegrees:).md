

- Foundation
- NSAffineTransform
-  rotate(byDegrees:) 

Instance Method

# rotate(byDegrees:)

Applies a rotation factor (measured in degrees) to the receiver’s transformation matrix.

Mac Catalyst 13.0+macOS 10.0+

``` source
func rotate(byDegrees angle: Double)
```

## Parameters 

`angle`  

The rotation angle, measured in degrees.

## Discussion

After invoking this method, applying the receiver’s matrix turns the axes counterclockwise about the current origin by `angle` degrees, in addition to performing all previous transformations.

## See Also

### Accumulating Transformations

func rotate(byRadians: Double)

Applies a rotation factor (measured in radians) to the receiver’s transformation matrix.

func scale(by: Double)

Applies the specified scaling factor along both x and y axes to the receiver’s transformation matrix.

func scaleX(by: Double, yBy: Double)

Applies scaling factors to each axis of the receiver’s transformation matrix.

func translateX(by: Double, yBy: Double)

Applies the specified translation factors to the receiver’s transformation matrix.

func append(NSAffineTransform)

Appends the specified matrix to the receiver’s matrix.

func prepend(NSAffineTransform)

Prepends the specified matrix to the receiver’s matrix.

func invert()

Replaces the receiver’s matrix with its inverse matrix.

