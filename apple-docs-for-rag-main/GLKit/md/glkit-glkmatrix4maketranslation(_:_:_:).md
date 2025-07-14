

- GLKit
-  GLKMatrix4MakeTranslation(\_:\_:\_:) 

Function

# GLKMatrix4MakeTranslation(\_:\_:\_:)

Returns a `4x4` matrix that performs a translation.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKMatrix4MakeTranslation(
    _ tx: Float,
    _ ty: Float,
    _ tz: Float
) -> GLKMatrix4
```

## Parameters 

`tx`  

The amount to translate the `x` component.

`ty`  

The amount to translate the `y` component.

`tz`  

The amount to translate the `z` component.

## Return Value

A new translation matrix.

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

func GLKMatrix4MakeLookAt(Float, Float, Float, Float, Float, Float, Float, Float, Float) -> GLKMatrix4

Returns a `4x4` matrix that transforms world coordinates to eye coordinates.

func GLKMatrix4MakeOrtho(Float, Float, Float, Float, Float, Float) -> GLKMatrix4

Returns a `4x4` orthographic projection matrix.

func GLKMatrix4MakePerspective(Float, Float, Float, Float) -> GLKMatrix4

Returns a `4x4` perspective projection matrix.

