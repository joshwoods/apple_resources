

- Foundation
- NSAffineTransform
-  prepend(\_:) 

Instance Method

# prepend(\_:)

Prepends the specified matrix to the receiver’s matrix.

Mac Catalyst 13.0+macOS 10.0+

**Mac Catalyst**

``` source
func prepend(_ transform: NSAffineTransform)
```

**macOS**

``` source
func prepend(_ transform: AffineTransform)
```

## Parameters 

`transform`  

The matrix to prepend to the receiver.

## Discussion

This method multiplies the matrix in `transform` by the receiver’s matrix and replaces the receiver’s matrix with the result. This type of operation is the same as applying the transformations in `transform` followed by the transformations in the receiver.

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

func invert()

Replaces the receiver’s matrix with its inverse matrix.

