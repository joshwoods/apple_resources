

- GLKit
-  GLKQuaternionSlerp(\_:\_:\_:) 

Function

# GLKQuaternionSlerp(\_:\_:\_:)

Returns the spherical linear interpolation of two quaternions.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKQuaternionSlerp(
    _ quaternionStart: GLKQuaternion,
    _ quaternionEnd: GLKQuaternion,
    _ t: Float
) -> GLKQuaternion
```

## Parameters 

`quaternionStart`  

The starting point.

`quaternionEnd`  

The ending point.

`t`  

The interpolation factor.

## Return Value

A new quaternion. When `t=0`, the result is the start quaternion. When `t=1.0`, the result is the end quaternion. For any other value of `t`, the result is a spherical linear interpolation between the two quaternions.

## See Also

### Performing Mathematical Operations on Quaternions

func GLKQuaternionNormalize(GLKQuaternion) -> GLKQuaternion

Returns a normalized version of a quaternion.

func GLKQuaternionInvert(GLKQuaternion) -> GLKQuaternion

Returns an inverse of a quaternion.

func GLKQuaternionConjugate(GLKQuaternion) -> GLKQuaternion

Returns the conjugate of a quaternion.

func GLKQuaternionAdd(GLKQuaternion, GLKQuaternion) -> GLKQuaternion

Returns the sum of two quaternions.

func GLKQuaternionSubtract(GLKQuaternion, GLKQuaternion) -> GLKQuaternion

Returns the difference between two quaternions.

func GLKQuaternionMultiply(GLKQuaternion, GLKQuaternion) -> GLKQuaternion

Returns the product of two quaternions.

