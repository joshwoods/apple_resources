

- GLKit
-  GLKMatrix4InvertAndTranspose(\_:\_:) 

Function

# GLKMatrix4InvertAndTranspose(\_:\_:)

Returns the inverse transpose of a matrix.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKMatrix4InvertAndTranspose(
    _ matrix: GLKMatrix4,
    _ isInvertible: UnsafeMutablePointer?
) -> GLKMatrix4
```

## Parameters 

`matrix`  

A `4x4` matrix.

`isInvertible`  

On return, this holds true if the matrix was inverted or false if the matrix is not invertible.

## Return Value

If `isInvertible` was set to true, this holds an inverted and transposed matrix. Otherwise, the identity matrix is returned.

## See Also

### Performing Mathematical Operations on Matrices

func GLKMatrix4Invert(GLKMatrix4, UnsafeMutablePointer&lt;Bool>?) -> GLKMatrix4

Returns the inverse of a matrix.

func GLKMatrix4Transpose(GLKMatrix4) -> GLKMatrix4

Returns the transpose of a matrix.

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

func GLKMatrix4Translate(GLKMatrix4, Float, Float, Float) -> GLKMatrix4

Returns a new `4x4` matrix created by concatenating a matrix with a translation transform.

func GLKMatrix4TranslateWithVector3(GLKMatrix4, GLKVector3) -> GLKMatrix4

Returns a new `4x4` matrix created by concatenating a matrix with a translation transform defined by a vector.

func GLKMatrix4TranslateWithVector4(GLKMatrix4, GLKVector4) -> GLKMatrix4

Returns a new `4x4` matrix created by concatenating a matrix with a translation transform defined by a vector.

