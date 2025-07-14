

- Foundation
- AffineTransform
-  translate(x:y:) 

Instance Method

# translate(x:y:)

Mutates an affine transformation matrix to perform the specified translation.

iOS 8.0+iPadOS 8.0+macOS 10.10+tvOS 9.0+watchOS 2.0+

``` source
mutating func translate(
    x: CGFloat,
    y: CGFloat
)
```

## Parameters 

`x`  

The horizontal translation value.

`y`  

The vertical translation value.

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

func append(AffineTransform)

Mutates an affine transformation by appending another affine transform.

func prepend(AffineTransform)

Mutates an affine transformation by prepending another affine transform.

func invert()

Inverts the transformation matrix, if possible.

func inverted() -> AffineTransform?

Returns an inverted version of the matrix, if possible, or nil if not.

