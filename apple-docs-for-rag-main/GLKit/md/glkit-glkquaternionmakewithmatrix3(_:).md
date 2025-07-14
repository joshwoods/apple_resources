

- GLKit
-  GLKQuaternionMakeWithMatrix3(\_:) 

Function

# GLKQuaternionMakeWithMatrix3(\_:)

Creates a quaternion from a rotation matrix.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKQuaternionMakeWithMatrix3(_ matrix: GLKMatrix3) -> GLKQuaternion
```

## Parameters 

`matrix`  

A rotation matrix to convert into a quaternion.

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

func GLKQuaternionMakeWithAngleAndVector3Axis(Float, GLKVector3) -> GLKQuaternion

Creates a quaternion that represents a rotation around an axis.

func GLKQuaternionMakeWithMatrix4(GLKMatrix4) -> GLKQuaternion

Creates a quaternion from a rotation matrix.

