

- GLKit
-  GLKQuaternionConjugate(\_:) 

Function

# GLKQuaternionConjugate(\_:)

Returns the conjugate of a quaternion.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKQuaternionConjugate(_ quaternion: GLKQuaternion) -> GLKQuaternion
```

## Parameters 

`quaternion`  

A quaternion.

## Return Value

A new quaternion that is the conjugate of the source quaternion.

## Discussion

The conjugate of a quaternion has the same scalar value, but the signs of the vector components are flipped.

## See Also

### Performing Mathematical Operations on Quaternions

func GLKQuaternionNormalize(GLKQuaternion) -> GLKQuaternion

Returns a normalized version of a quaternion.

func GLKQuaternionInvert(GLKQuaternion) -> GLKQuaternion

Returns an inverse of a quaternion.

func GLKQuaternionAdd(GLKQuaternion, GLKQuaternion) -> GLKQuaternion

Returns the sum of two quaternions.

func GLKQuaternionSubtract(GLKQuaternion, GLKQuaternion) -> GLKQuaternion

Returns the difference between two quaternions.

func GLKQuaternionMultiply(GLKQuaternion, GLKQuaternion) -> GLKQuaternion

Returns the product of two quaternions.

func GLKQuaternionSlerp(GLKQuaternion, GLKQuaternion, Float) -> GLKQuaternion

Returns the spherical linear interpolation of two quaternions.

