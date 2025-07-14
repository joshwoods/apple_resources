

- GLKit
-  GLKit Functions 

API Collection

# GLKit Functions

## Topics

### Functions

func GLKMatrixStackCreate(CFAllocator?) -> Unmanaged&lt;GLKMatrixStack>?

Allocates and returns a new matrix stack.

func GLKMatrixStackGetMatrix2(GLKMatrixStack) -> GLKMatrix2

Returns the top-left `2x2` corner of the top matrix.

func GLKMatrixStackGetMatrix3(GLKMatrixStack) -> GLKMatrix3

Returns the top-left `3x3` corner of the top matrix.

func GLKMatrixStackGetMatrix3Inverse(GLKMatrixStack) -> GLKMatrix3

Fetches the top-left `3x3` corner of the top matrix and returns its inverse.

func GLKMatrixStackGetMatrix3InverseTranspose(GLKMatrixStack) -> GLKMatrix3

Fetches the top-left `3x3` corner of the top matrix and returns its inverse transpose.

func GLKMatrixStackGetMatrix4(GLKMatrixStack) -> GLKMatrix4

Returns a copy of the top matrix on the stack.

func GLKMatrixStackGetMatrix4Inverse(GLKMatrixStack) -> GLKMatrix4

Returns the inverse of the top matrix.

func GLKMatrixStackGetMatrix4InverseTranspose(GLKMatrixStack) -> GLKMatrix4

Returns the inverse transpose of the top matrix.

func GLKMatrixStackGetTypeID() -> CFTypeID

Returns the Core Foundation type for a matrix stack.

func GLKMatrixStackLoadMatrix4(GLKMatrixStack, GLKMatrix4)

Replaces the contents of the top matrix with a new matrix.

func GLKMatrixStackMultiplyMatrix4(GLKMatrixStack, GLKMatrix4)

Replaces the contents of the top matrix with a matrix calculated by multiplying the contents of the top matrix by another matrix.

func GLKMatrixStackMultiplyMatrixStack(GLKMatrixStack, GLKMatrixStack)

Replaces the contents of the top matrix with a matrix calculated by multiplying the contents of the top matrix by the top matrix of another matrix stack.

func GLKMatrixStackPop(GLKMatrixStack)

Removes the topmost entry from the stack.

func GLKMatrixStackPush(GLKMatrixStack)

Push a copy of the topmost matrix onto the top of the stack.

func GLKMatrixStackRotate(GLKMatrixStack, Float, Float, Float, Float)

Replaces the contents of the top matrix with a matrix calculated by composing the top matrix with a rotation around an arbitrary axis.

func GLKMatrixStackRotateWithVector3(GLKMatrixStack, Float, GLKVector3)

Replaces the contents of the top matrix with a matrix calculated by composing the top matrix with a rotation around an arbitrary axis.

func GLKMatrixStackRotateWithVector4(GLKMatrixStack, Float, GLKVector4)

Replaces the contents of the top matrix with a matrix calculated by composing the top matrix with a rotation around an arbitrary axis.

func GLKMatrixStackRotateX(GLKMatrixStack, Float)

Replaces the contents of the top matrix with a matrix calculated by composing the top matrix with a rotation around the positive-x axis.

func GLKMatrixStackRotateY(GLKMatrixStack, Float)

Replaces the contents of the top matrix with a matrix calculated by composing the top matrix with a rotation around the positive-y axis.

func GLKMatrixStackRotateZ(GLKMatrixStack, Float)

Replaces the contents of the top matrix with a matrix calculated by composing the top matrix with a rotation around the positive-z axis.

func GLKMatrixStackScale(GLKMatrixStack, Float, Float, Float)

Replaces the contents of the top matrix with a matrix calculated by scaling the contents of the top matrix.

func GLKMatrixStackScaleWithVector3(GLKMatrixStack, GLKVector3)

Replaces the contents of the top matrix with a matrix calculated by composing the top matrix with a scaling operation.

func GLKMatrixStackScaleWithVector4(GLKMatrixStack, GLKVector4)

Replaces the contents of the top matrix with a matrix calculated by composing the top matrix with a scaling operation defined by a vector.

func GLKMatrixStackSize(GLKMatrixStack) -> Int32

Returns the number of matrices present on the matrix stack.

func GLKMatrixStackTranslate(GLKMatrixStack, Float, Float, Float)

Replaces the contents of the top matrix with a matrix calculated by composing the top matrix with a translation operation.

func GLKMatrixStackTranslateWithVector3(GLKMatrixStack, GLKVector3)

Replaces the contents of the top matrix with a matrix calculated by composing the top matrix with a translation defined by a vector.

func GLKMatrixStackTranslateWithVector4(GLKMatrixStack, GLKVector4)

Replaces the contents of the top matrix with a matrix calculated by composing the top matrix with a translation defined by a vector.

func GLKVertexAttributeParametersFromModelIO(MDLVertexFormat) -> GLKVertexAttributeParameters

## See Also

### Reference

GLKit Structures

GLKit Enumerations

GLKit Constants

GLKit Data Types

