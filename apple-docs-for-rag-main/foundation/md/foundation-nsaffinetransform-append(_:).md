

- Foundation
- NSAffineTransform
-  append(\_:) 

Instance Method

# append(\_:)

Appends the specified matrix to the receiver’s matrix.

Mac Catalyst 13.0+macOS 10.0+

**macOS**

``` source
func append(_ transform: AffineTransform)
```

**Mac Catalyst**

``` source
func append(_ transform: NSAffineTransform)
```

## Parameters 

`transform`  

The matrix to append to the receiver.

## Discussion

This method multiplies the receiver’s matrix by the matrix in `aTransform` and replaces the receiver’s matrix with the results. This type of operation is the same as applying the transformations in the receiver followed by the transformations in `aTransform`.

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

func prepend(NSAffineTransform)

Prepends the specified matrix to the receiver’s matrix.

func invert()

Replaces the receiver’s matrix with its inverse matrix.

