

- GLKit
-  GLKQuaternionNormalize(\_:) 

Function

# GLKQuaternionNormalize(\_:)

Returns a normalized version of a quaternion.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKQuaternionNormalize(_ quaternion: GLKQuaternion) -> GLKQuaternion
```

## Parameters 

`quaternion`  

A quaternion.

## Return Value

A new quaternion, normalized to have a length of `1.0`.

## See Also

### Performing Mathematical Operations on Quaternions

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

func GLKQuaternionSlerp(GLKQuaternion, GLKQuaternion, Float) -> GLKQuaternion

Returns the spherical linear interpolation of two quaternions.

