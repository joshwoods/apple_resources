

- GLKit
-  GLKMatrix3MakeWithQuaternion(\_:) 

Function

# GLKMatrix3MakeWithQuaternion(\_:)

Returns a `3x3` matrix that performs a rotation based on a quaternion.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKMatrix3MakeWithQuaternion(_ quaternion: GLKQuaternion) -> GLKMatrix3
```

## Parameters 

`quaternion`  

The quaternion.

## Return Value

A new matrix that provides an equivalent rotation to that stored in the quaternion.

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

func GLKMatrix3MakeRotation(Float, Float, Float, Float) -> GLKMatrix3

Returns a `3x3` matrix that performs a rotation around an arbitrary vector.

func GLKMatrix3MakeXRotation(Float) -> GLKMatrix3

Returns a `3x3` matrix that performs a rotation around the positive x-axis.

func GLKMatrix3MakeYRotation(Float) -> GLKMatrix3

Returns a `3x3` matrix that performs a rotation around the positive y-axis.

func GLKMatrix3MakeZRotation(Float) -> GLKMatrix3

Returns a `3x3` matrix that performs a rotation around the positive z-axis.

func GLKMatrix3MakeScale(Float, Float, Float) -> GLKMatrix3

Returns a `3x3` matrix that performs a scaling transformation.

