

- Foundation
- AffineTransform
-  init(scale:) 

Initializer

# init(scale:)

Creates an affine transformation matrix from scaling a single value.

iOS 8.0+iPadOS 8.0+macOS 10.10+tvOS 9.0+watchOS 2.0+

``` source
init(scale factor: CGFloat)
```

## Parameters 

`factor`  

The scale factor.

## Discussion

The matrix takes the following form:

```
[ f  0  0 ]
[ 0  f  0 ]
[ 0  0  1 ]
```

## See Also

### Creating Transforms

init()

Creates an affine transformation matrix with identity values.

init(rotationByDegrees: CGFloat)

Creates an affine transformation matrix from a rotation angle.

init(rotationByRadians: CGFloat)

Creates an affine transformation matrix from a rotation angle.

init(scaleByX: CGFloat, byY: CGFloat)

Creates an affine transformation matrix from scaling values.

init(translationByX: CGFloat, byY: CGFloat)

Creates an affine transformation matrix from translation values.

init(m11: CGFloat, m12: CGFloat, m21: CGFloat, m22: CGFloat, tX: CGFloat, tY: CGFloat)

Creates an affine transformation.

