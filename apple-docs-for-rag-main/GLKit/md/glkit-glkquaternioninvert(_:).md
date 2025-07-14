

- GLKit
-  GLKQuaternionInvert(\_:) 

Function

# GLKQuaternionInvert(\_:)

Returns an inverse of a quaternion.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKQuaternionInvert(_ quaternion: GLKQuaternion) -> GLKQuaternion
```

## Parameters 

`quaternion`  

A quaternion.

## Return Value

A new quaternion that is the inverse of the source quaternion.

## See Also

### Performing Mathematical Operations on Quaternions

func GLKQuaternionNormalize(GLKQuaternion) -> GLKQuaternion

Returns a normalized version of a quaternion.

func GLKQuaternionConjugate(GLKQuaternion) -> GLKQuaternion

Returns the conjugate of a quaternion.

func GLKQuaternionAdd(GLKQuaternion, GLKQuaternion) -> GLKQuaternion

Returns the sum of two quaternions.

func GLKQuaternionSubtract(GLKQuaternion, GLKQuaternion) -> GLKQuaternion

Returns the difference between two quaternions.

func GLKQuaternionMultiply(GLKQuaternion, GLKQuaternion) -> GLKQuaternion

Returns the product of two quaternions.

func GLKQuaternionSlerp(GLKQuaternion, GLKQuaternion, Float) -> GLKQuaternion

Returns the spherical linear interpolation of two quaternions.

