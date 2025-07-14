

- GLKit
-  GLKQuaternionMakeWithAngleAndVector3Axis(\_:\_:) 

Function

# GLKQuaternionMakeWithAngleAndVector3Axis(\_:\_:)

Creates a quaternion that represents a rotation around an axis.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKQuaternionMakeWithAngleAndVector3Axis(
    _ radians: Float,
    _ axisVector: GLKVector3
) -> GLKQuaternion
```

## Parameters 

`radians`  

The angle of the rotation in radians (a positive angle is counterclockwise).

`axisVector`  

The axis of rotation.

## Return Value

A new quaternion.

## See Also

### Creating Quaternions

func GLKQuaternionMake(Float, Float, Float, Float) -> GLKQuaternion

Returns a quaternion created from its separate components.

func GLKQuaternionMakeWithArray(UnsafeMutablePointer&lt;Float>!) -> GLKQuaternion

Returns a quaternion created from an array of components.

func GLKQuaternionMakeWithVector3(GLKVector3, Float) -> GLKQuaternion

Returns a quaternion created from a vector and a scalar.

func GLKQuaternionMakeWithAngleAndAxis(Float, Float, Float, Float) -> GLKQuaternion

Creates a quaternion that represents a rotation around an axis.

func GLKQuaternionMakeWithMatrix3(GLKMatrix3) -> GLKQuaternion

Creates a quaternion from a rotation matrix.

func GLKQuaternionMakeWithMatrix4(GLKMatrix4) -> GLKQuaternion

Creates a quaternion from a rotation matrix.

