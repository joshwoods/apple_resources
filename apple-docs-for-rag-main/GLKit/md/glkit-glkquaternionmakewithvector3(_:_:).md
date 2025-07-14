

- GLKit
-  GLKQuaternionMakeWithVector3(\_:\_:) 

Function

# GLKQuaternionMakeWithVector3(\_:\_:)

Returns a quaternion created from a vector and a scalar.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKQuaternionMakeWithVector3(
    _ vector: GLKVector3,
    _ scalar: Float
) -> GLKQuaternion
```

## Parameters 

`vector`  

The vector portion of the new quaternion.

`scalar`  

The scalar portion of the new quaternion.

## Return Value

A new quaternion.

## See Also

### Creating Quaternions

func GLKQuaternionMake(Float, Float, Float, Float) -> GLKQuaternion

Returns a quaternion created from its separate components.

func GLKQuaternionMakeWithArray(UnsafeMutablePointer&lt;Float>!) -> GLKQuaternion

Returns a quaternion created from an array of components.

func GLKQuaternionMakeWithAngleAndAxis(Float, Float, Float, Float) -> GLKQuaternion

Creates a quaternion that represents a rotation around an axis.

func GLKQuaternionMakeWithAngleAndVector3Axis(Float, GLKVector3) -> GLKQuaternion

Creates a quaternion that represents a rotation around an axis.

func GLKQuaternionMakeWithMatrix3(GLKMatrix3) -> GLKQuaternion

Creates a quaternion from a rotation matrix.

func GLKQuaternionMakeWithMatrix4(GLKMatrix4) -> GLKQuaternion

Creates a quaternion from a rotation matrix.

