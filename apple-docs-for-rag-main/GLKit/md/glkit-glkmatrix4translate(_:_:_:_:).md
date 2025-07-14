

- GLKit
-  GLKMatrix4Translate(\_:\_:\_:\_:) 

Function

# GLKMatrix4Translate(\_:\_:\_:\_:)

Returns a new `4x4` matrix created by concatenating a matrix with a translation transform.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKMatrix4Translate(
    _ matrix: GLKMatrix4,
    _ tx: Float,
    _ ty: Float,
    _ tz: Float
) -> GLKMatrix4
```

## Parameters 

`matrix`  

A matrix.

`tx`  

The amount to translate the `x` component.

`ty`  

The amount to translate the `y` component.

`tz`  

The amount to translate the `z` component.

## Return Value

A new matrix.

## See Also

### Performing Mathematical Operations on Matrices

func GLKMatrix4Invert(GLKMatrix4, UnsafeMutablePointer&lt;Bool>?) -> GLKMatrix4

Returns the inverse of a matrix.

func GLKMatrix4Transpose(GLKMatrix4) -> GLKMatrix4

Returns the transpose of a matrix.

func GLKMatrix4InvertAndTranspose(GLKMatrix4, UnsafeMutablePointer&lt;Bool>?) -> GLKMatrix4

Returns the inverse transpose of a matrix.

func GLKMatrix4Multiply(GLKMatrix4, GLKMatrix4) -> GLKMatrix4

Returns the product of two matrices.

func GLKMatrix4Rotate(GLKMatrix4, Float, Float, Float, Float) -> GLKMatrix4

Returns a new `4x4` matrix created by concatenating a matrix with a rotation around a vector.

func GLKMatrix4RotateWithVector3(GLKMatrix4, Float, GLKVector3) -> GLKMatrix4

Returns a new `4x4` matrix created by concatenating a matrix with a rotation around a vector.

func GLKMatrix4RotateWithVector4(GLKMatrix4, Float, GLKVector4) -> GLKMatrix4

Returns a new `4x4` matrix created by concatenating a matrix with a rotation around a vector.

func GLKMatrix4RotateX(GLKMatrix4, Float) -> GLKMatrix4

Returns a new `4x4` matrix created by concatenating a matrix with a rotation around the x-axis.

func GLKMatrix4RotateY(GLKMatrix4, Float) -> GLKMatrix4

Returns a new `4x4` matrix created by concatenating a matrix with a rotation around the y-axis.

func GLKMatrix4RotateZ(GLKMatrix4, Float) -> GLKMatrix4

Returns a new `4x4` matrix created by concatenating a matrix with a rotation around the z-axis.

func GLKMatrix4Scale(GLKMatrix4, Float, Float, Float) -> GLKMatrix4

Returns a new `4x4` matrix created by concatenating a matrix with a scaling transform.

func GLKMatrix4ScaleWithVector3(GLKMatrix4, GLKVector3) -> GLKMatrix4

Returns a new `4x4` matrix created by concatenating a matrix with a scaling transform defined by a vector.

func GLKMatrix4ScaleWithVector4(GLKMatrix4, GLKVector4) -> GLKMatrix4

Returns a new `4x4` matrix created by concatenating a matrix with a scaling transform defined by a vector.

func GLKMatrix4TranslateWithVector3(GLKMatrix4, GLKVector3) -> GLKMatrix4

Returns a new `4x4` matrix created by concatenating a matrix with a translation transform defined by a vector.

func GLKMatrix4TranslateWithVector4(GLKMatrix4, GLKVector4) -> GLKMatrix4

Returns a new `4x4` matrix created by concatenating a matrix with a translation transform defined by a vector.

