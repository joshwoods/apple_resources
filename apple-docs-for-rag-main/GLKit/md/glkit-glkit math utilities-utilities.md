

- GLKit
-  GLKit Math Utilities 

API Collection

# GLKit Math Utilities

## Overview

Math routines without a specific type associated with them.

## Topics

### Converting Angles

func GLKMathDegreesToRadians(Float) -> Float

Converts an angle measured in degrees to radians.

func GLKMathRadiansToDegrees(Float) -> Float

Converts an angle measured in radians to degrees.

### Projecting Vectors

func GLKMathProject(GLKVector3, GLKMatrix4, GLKMatrix4, UnsafeMutablePointer&lt;Int32>) -> GLKVector3

Projects a point in object space into the window coordinate system.

func GLKMathUnproject(GLKVector3, GLKMatrix4, GLKMatrix4, UnsafeMutablePointer&lt;Int32>, UnsafeMutablePointer&lt;Bool>?) -> GLKVector3

Projects a point in view space into object space.

### Obtaining String Descriptions

func NSStringFromGLKMatrix2(GLKMatrix2) -> String

Returns a string that represents the contents of a matrix.

func NSStringFromGLKMatrix3(GLKMatrix3) -> String

Returns a string that represents the contents of a matrix.

func NSStringFromGLKMatrix4(GLKMatrix4) -> String

Returns a string that represents the contents of a matrix.

func NSStringFromGLKVector2(GLKVector2) -> String

Returns a string that represents the contents of a vector.

func NSStringFromGLKVector3(GLKVector3) -> String

Returns a string that represents the contents of a vector.

func NSStringFromGLKVector4(GLKVector4) -> String

Returns a string that represents the contents of a vector.

func NSStringFromGLKQuaternion(GLKQuaternion) -> String

Returns a string that represents the contents of a quaternion.

## See Also

### Math Utilties

class GLKMatrixStack

An opaque type that represents a stack of 4 x 4 matrices, providing support for hierarchical transform modeling and similar tasks.

GLKMatrix3

GLKMatrix4

GLKVector2

GLKVector3

GLKVector4

GLKQuaternion

