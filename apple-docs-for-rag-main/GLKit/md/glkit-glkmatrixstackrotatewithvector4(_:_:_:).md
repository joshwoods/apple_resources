

- GLKit
-  GLKMatrixStackRotateWithVector4(\_:\_:\_:) 

Function

# GLKMatrixStackRotateWithVector4(\_:\_:\_:)

Replaces the contents of the top matrix with a matrix calculated by composing the top matrix with a rotation around an arbitrary axis.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKMatrixStackRotateWithVector4(
    _ stack: GLKMatrixStack,
    _ radians: Float,
    _ axisVector: GLKVector4
)
```

## Parameters 

`stack`  

A matrix stack.

`radians`  

The angle of the rotation (a positive angle is counterclockwise).

`axisVector`  

A vector whose `x`,`y` and `z` coordinates are used as the axis of rotation.

## See Also

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

