

- GLKit
-  GLKQuaternionMake(\_:\_:\_:\_:) 

Function

# GLKQuaternionMake(\_:\_:\_:\_:)

Returns a quaternion created from its separate components.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKQuaternionMake(
    _ x: Float,
    _ y: Float,
    _ z: Float,
    _ w: Float
) -> GLKQuaternion
```

## Parameters 

`x`  

The `x` component of the quaternion.

`y`  

The `y` component of the quaternion.

`z`  

The `z` component of the quaternion.

`w`  

The `w` component of the quaternion.

## Return Value

A new quaternion.

## See Also

### Creating Quaternions

func GLKQuaternionMakeWithArray(UnsafeMutablePointer&lt;Float>!) -> GLKQuaternion

Returns a quaternion created from an array of components.

func GLKQuaternionMakeWithVector3(GLKVector3, Float) -> GLKQuaternion

Returns a quaternion created from a vector and a scalar.

func GLKQuaternionMakeWithAngleAndAxis(Float, Float, Float, Float) -> GLKQuaternion

Creates a quaternion that represents a rotation around an axis.

func GLKQuaternionMakeWithAngleAndVector3Axis(Float, GLKVector3) -> GLKQuaternion

Creates a quaternion that represents a rotation around an axis.

func GLKQuaternionMakeWithMatrix3(GLKMatrix3) -> GLKQuaternion

Creates a quaternion from a rotation matrix.

func GLKQuaternionMakeWithMatrix4(GLKMatrix4) -> GLKQuaternion

Creates a quaternion from a rotation matrix.

