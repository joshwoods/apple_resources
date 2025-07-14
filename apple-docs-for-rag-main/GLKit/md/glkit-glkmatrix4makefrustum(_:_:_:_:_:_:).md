

- GLKit
-  GLKMatrix4MakeFrustum(\_:\_:\_:\_:\_:\_:) 

Function

# GLKMatrix4MakeFrustum(\_:\_:\_:\_:\_:\_:)

Returns a `4x4` perspective projection matrix.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKMatrix4MakeFrustum(
    _ left: Float,
    _ right: Float,
    _ bottom: Float,
    _ top: Float,
    _ nearZ: Float,
    _ farZ: Float
) -> GLKMatrix4
```

## Parameters 

`left`  

The left clipping plane.

`right`  

The right clipping plane.

`bottom`  

The bottom clipping plane.

`top`  

The top clipping plane.

`nearZ`  

The near clipping distance. Must be positive.

`farZ`  

The far clipping distance. Must be positive and greater than the near distance.

## Return Value

A projection matrix.

## Discussion

This function creates the same orthographic projection matrix previously provided in OpenGL ES 1.1 by the `glFrustum` function.

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

func GLKMatrix4MakeLookAt(Float, Float, Float, Float, Float, Float, Float, Float, Float) -> GLKMatrix4

Returns a `4x4` matrix that transforms world coordinates to eye coordinates.

func GLKMatrix4MakeOrtho(Float, Float, Float, Float, Float, Float) -> GLKMatrix4

Returns a `4x4` orthographic projection matrix.

