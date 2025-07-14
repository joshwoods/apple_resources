

- Foundation
- AffineTransform
-  invert() 

Instance Method

# invert()

Inverts the transformation matrix, if possible.

iOS 8.0+iPadOS 8.0+macOS 10.10+tvOS 9.0+watchOS 2.0+

``` source
mutating func invert()
```

## Discussion

Matrices with a determinant less than the smallest valid representation of a double value and greater than zero are invalid for representing as an inverse. If this can potentially happen to the input transform, use the inverted() method instead. The inverted() method returns `nil` if the function can’t reliably invert the matrix.

You can calculate the determinant using the following formula:

```
D = (m11 * m22) - (m12 * m21)
```

## See Also

### Accumulating Tranformations

func rotate(byDegrees: CGFloat)

Mutates an affine transformation matrix to apply a rotation.

func rotate(byRadians: CGFloat)

Mutates an affine transformation matrix to apply a rotation.

func scale(CGFloat)

Mutates an affine transformation matrix to apply scaling in both x and y dimensions.

func scale(x: CGFloat, y: CGFloat)

Mutates an affine transformation matrix to apply scaling in each of the x and y dimensions.

func translate(x: CGFloat, y: CGFloat)

Mutates an affine transformation matrix to perform the specified translation.

func append(AffineTransform)

Mutates an affine transformation by appending another affine transform.

func prepend(AffineTransform)

Mutates an affine transformation by prepending another affine transform.

func inverted() -> AffineTransform?

Returns an inverted version of the matrix, if possible, or nil if not.

