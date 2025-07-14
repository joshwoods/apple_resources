

- GLKit
-  GLKMatrix3Multiply(\_:\_:) 

Function

# GLKMatrix3Multiply(\_:\_:)

Returns the product of two matrices.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKMatrix3Multiply(
    _ matrixLeft: GLKMatrix3,
    _ matrixRight: GLKMatrix3
) -> GLKMatrix3
```

## Parameters 

`matrixLeft`  

The multiplicand.

`matrixRight`  

The multiplier.

## Return Value

A new matrix formed by multiplying the two matrices together.

## See Also

### Performing Mathematical Operations on Matrices

func GLKMatrix3Invert(GLKMatrix3, UnsafeMutablePointer&lt;Bool>!) -> GLKMatrix3

Returns the inverse of a matrix.

func GLKMatrix3Transpose(GLKMatrix3) -> GLKMatrix3

Returns the transpose of a matrix.

func GLKMatrix3InvertAndTranspose(GLKMatrix3, UnsafeMutablePointer&lt;Bool>!) -> GLKMatrix3

Returns the inverse transpose of a matrix.

func GLKMatrix3Rotate(GLKMatrix3, Float, Float, Float, Float) -> GLKMatrix3

Returns a new `3x3` matrix created by concatenating a matrix with a rotation around a vector.

func GLKMatrix3RotateWithVector3(GLKMatrix3, Float, GLKVector3) -> GLKMatrix3

Returns a new `3x3` matrix created by concatenating a matrix with a rotation around a vector.

func GLKMatrix3RotateWithVector4(GLKMatrix3, Float, GLKVector4) -> GLKMatrix3

Returns a new `3x3` matrix created by concatenating a matrix with a rotation around a vector.

func GLKMatrix3RotateX(GLKMatrix3, Float) -> GLKMatrix3

Returns a new `3x3` matrix created by concatenating a matrix with a rotation around the x-axis.

func GLKMatrix3RotateY(GLKMatrix3, Float) -> GLKMatrix3

Returns a new `3x3` matrix created by concatenating a matrix with a rotation around the y-axis.

func GLKMatrix3RotateZ(GLKMatrix3, Float) -> GLKMatrix3

Returns a new `3x3` matrix created by concatenating a matrix with a rotation around the z-axis.

func GLKMatrix3Scale(GLKMatrix3, Float, Float, Float) -> GLKMatrix3

Returns a new `3x3` matrix created by concatenating a matrix with a scaling transform.

func GLKMatrix3ScaleWithVector3(GLKMatrix3, GLKVector3) -> GLKMatrix3

Returns a new `3x3` matrix created by concatenating a matrix with a scaling transform defined by a vector.

func GLKMatrix3ScaleWithVector4(GLKMatrix3, GLKVector4) -> GLKMatrix3

Returns a new `3x3` matrix created by concatenating a matrix with a scaling transform defined by a vector.

func GLKMatrix3Add(GLKMatrix3, GLKMatrix3) -> GLKMatrix3

Returns a new `3x3` matrix created by performing a component-wise addition of two matrices.

func GLKMatrix3Subtract(GLKMatrix3, GLKMatrix3) -> GLKMatrix3

Returns a new `3x3` matrix created by performing a component-wise subtraction of two matrices.

