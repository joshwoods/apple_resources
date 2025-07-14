

- Foundation
- NSAffineTransform
-  invert() 

Instance Method

# invert()

Replaces the receiver’s matrix with its inverse matrix.

Mac Catalyst 13.0+macOS 10.0+

``` source
func invert()
```

## Discussion

Inverse matrices are useful for undoing the effects of a matrix. If a previous point (x,y) was transformed to (x’,y’), inverting the matrix and applying it to point (x’,y’) yields the point (x,y).

You can also use inverse matrices in conjunction with the concat() method to remove the effects of concatenating the matrix to the current transformation matrix of the current graphic context.

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

func translateX(by: Double, yBy: Double)

Applies the specified translation factors to the receiver’s transformation matrix.

func append(NSAffineTransform)

Appends the specified matrix to the receiver’s matrix.

func prepend(NSAffineTransform)

Prepends the specified matrix to the receiver’s matrix.

