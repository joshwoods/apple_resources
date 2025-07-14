

- GLKit
-  GLKMatrix4MakeLookAt(\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# GLKMatrix4MakeLookAt(\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Returns a `4x4` matrix that transforms world coordinates to eye coordinates.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKMatrix4MakeLookAt(
    _ eyeX: Float,
    _ eyeY: Float,
    _ eyeZ: Float,
    _ centerX: Float,
    _ centerY: Float,
    _ centerZ: Float,
    _ upX: Float,
    _ upY: Float,
    _ upZ: Float
) -> GLKMatrix4
```

## Parameters 

`eyeX`  

The `x` coordinate of the eye position.

`eyeY`  

The `y` coordinate of the eye position.

`eyeZ`  

The `z` coordinate of the point position.

`centerX`  

The `x` coordinate of the point being looked at.

`centerY`  

The `y` coordinate of the point being looked at.

`centerZ`  

The `z` coordinate of the point being looked at.

`upX`  

The `x` coordinate of the camera’s up vector.

`upY`  

The `y` coordinate of the camera’s up vector.

`upZ`  

The `z` coordinate of the camera’s up vector.

## Return Value

A newly initialized view matrix.

## Discussion

This function creates a matrix in a way similar to the `gluLookAt` function previously provided in OpenGL ES 1.1.

## See Also

### Creating Matrices

func GLKMatrix4Make(Float, Float, Float, Float, Float, Float, Float, Float, Float, Float, Float, Float, Float, Float, Float, Float) -> GLKMatrix4

Returns a `4x4` matrix created from individual component values.

func GLKMatrix4MakeAndTranspose(Float, Float, Float, Float, Float, Float, Float, Float, Float, Float, Float, Float, Float, Float, Float, Float) -> GLKMatrix4

Returns a `4x4` transposed matrix created from individual component values.

func GLKMatrix4MakeWithArray(UnsafeMutablePointer&lt;Float>!) -> GLKMatrix4

Returns a `4x4` matrix created from an array of component values.

func GLKMatrix4MakeWithArrayAndTranspose(UnsafeMutablePointer&lt;Float>!) -> GLKMatrix4

Returns a `4x4` transposed matrix created from an array of component values.

func GLKMatrix4MakeWithColumns(GLKVector4, GLKVector4, GLKVector4, GLKVector4) -> GLKMatrix4

Returns a `4x4` matrix created from four column vectors.

func GLKMatrix4MakeWithRows(GLKVector4, GLKVector4, GLKVector4, GLKVector4) -> GLKMatrix4

Returns a `4x4` matrix created from four row vectors.

func GLKMatrix4MakeRotation(Float, Float, Float, Float) -> GLKMatrix4

Returns a `4x4` matrix that performs a rotation around an arbitrary vector.

func GLKMatrix4MakeXRotation(Float) -> GLKMatrix4

Returns a `4x4` matrix that performs a rotation around the positive x-axis.

func GLKMatrix4MakeYRotation(Float) -> GLKMatrix4

Returns a `4x4` matrix that performs a rotation around the positive y-axis.

func GLKMatrix4MakeZRotation(Float) -> GLKMatrix4

Returns a `4x4` matrix that performs a rotation around the positive z-axis.

func GLKMatrix4MakeWithQuaternion(GLKQuaternion) -> GLKMatrix4

Returns a `4x4` matrix that performs a rotation based on a quaternion.

func GLKMatrix4MakeScale(Float, Float, Float) -> GLKMatrix4

Returns a `4x4` matrix that performs a scaling transformation.

func GLKMatrix4MakeTranslation(Float, Float, Float) -> GLKMatrix4

Returns a `4x4` matrix that performs a translation.

func GLKMatrix4MakeOrtho(Float, Float, Float, Float, Float, Float) -> GLKMatrix4

Returns a `4x4` orthographic projection matrix.

func GLKMatrix4MakePerspective(Float, Float, Float, Float) -> GLKMatrix4

Returns a `4x4` perspective projection matrix.

