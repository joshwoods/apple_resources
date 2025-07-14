

- GLKit
-  GLKQuaternionMakeWithArray(\_:) 

Function

# GLKQuaternionMakeWithArray(\_:)

Returns a quaternion created from an array of components.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKQuaternionMakeWithArray(_ values: UnsafeMutablePointer!) -> GLKQuaternion
```

## Parameters 

`values`  

The four components that comprise the new quaternion.

## Return Value

A new quaternion.

## See Also

### Creating Quaternions

func GLKQuaternionMake(Float, Float, Float, Float) -> GLKQuaternion

Returns a quaternion created from its separate components.

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

