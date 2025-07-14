

- Foundation
- AffineTransform
-  init(translationByX:byY:) 

Initializer

# init(translationByX:byY:)

Creates an affine transformation matrix from translation values.

iOS 8.0+iPadOS 8.0+macOS 10.10+tvOS 9.0+watchOS 2.0+

``` source
init(
    translationByX x: CGFloat,
    byY y: CGFloat
)
```

## Parameters 

`x`  

The horizontal translation value.

`y`  

The vertical translation value.

## Discussion

The matrix takes the following form:

```
[ 1  0  0 ]
[ 0  1  0 ]
[ x  y  1 ]
```

## See Also

### Creating Transforms

init()

Creates an affine transformation matrix with identity values.

init(rotationByDegrees: CGFloat)

Creates an affine transformation matrix from a rotation angle.

init(rotationByRadians: CGFloat)

Creates an affine transformation matrix from a rotation angle.

init(scale: CGFloat)

Creates an affine transformation matrix from scaling a single value.

init(scaleByX: CGFloat, byY: CGFloat)

Creates an affine transformation matrix from scaling values.

init(m11: CGFloat, m12: CGFloat, m21: CGFloat, m22: CGFloat, tX: CGFloat, tY: CGFloat)

Creates an affine transformation.

