

- GLKit
-  GLKMatrix3MakeRotation(\_:\_:\_:\_:) 

Function

# GLKMatrix3MakeRotation(\_:\_:\_:\_:)

Returns a `3x3` matrix that performs a rotation around an arbitrary vector.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKMatrix3MakeRotation(
    _ radians: Float,
    _ x: Float,
    _ y: Float,
    _ z: Float
) -> GLKMatrix3
```

## Parameters 

`radians`  

The angle of the rotation (a positive angle is counterclockwise).

`x`  

The `x` component of the rotation vector.

`y`  

The `y` component of the rotation vector.

`z`  

The `z` component of the rotation vector.

## Return Value

A new rotation matrix.

## See Also

### Creating Matrices

func GLKMatrix3Make(Float, Float, Float, Float, Float, Float, Float, Float, Float) -> GLKMatrix3

Returns a `3x3` matrix created from individual component values.

func GLKMatrix3MakeAndTranspose(Float, Float, Float, Float, Float, Float, Float, Float, Float) -> GLKMatrix3

Returns a `3x3` transposed matrix created from individual component values.

func GLKMatrix3MakeWithArray(UnsafeMutablePointer&lt;Float>!) -> GLKMatrix3

Returns a `3x3` matrix created from an array of component values.

func GLKMatrix3MakeWithArrayAndTranspose(UnsafeMutablePointer&lt;Float>!) -> GLKMatrix3

Returns a `3x3` transposed matrix created from an array of component values.

func GLKMatrix3MakeWithColumns(GLKVector3, GLKVector3, GLKVector3) -> GLKMatrix3

Returns a `3x3` matrix created from three column vectors.

func GLKMatrix3MakeWithRows(GLKVector3, GLKVector3, GLKVector3) -> GLKMatrix3

Returns a `3x3` matrix created from three row vectors.

func GLKMatrix3MakeXRotation(Float) -> GLKMatrix3

Returns a `3x3` matrix that performs a rotation around the positive x-axis.

func GLKMatrix3MakeYRotation(Float) -> GLKMatrix3

Returns a `3x3` matrix that performs a rotation around the positive y-axis.

func GLKMatrix3MakeZRotation(Float) -> GLKMatrix3

Returns a `3x3` matrix that performs a rotation around the positive z-axis.

func GLKMatrix3MakeWithQuaternion(GLKQuaternion) -> GLKMatrix3

Returns a `3x3` matrix that performs a rotation based on a quaternion.

func GLKMatrix3MakeScale(Float, Float, Float) -> GLKMatrix3

Returns a `3x3` matrix that performs a scaling transformation.

