

- GLKit
-  GLKQuaternionSubtract(\_:\_:) 

Function

# GLKQuaternionSubtract(\_:\_:)

Returns the difference between two quaternions.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKQuaternionSubtract(
    _ quaternionLeft: GLKQuaternion,
    _ quaternionRight: GLKQuaternion
) -> GLKQuaternion
```

## Parameters 

`quaternionLeft`  

The minuend.

`quaternionRight`  

The subtrahend.

## Return Value

A new quaternion.

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

func GLKQuaternionMultiply(GLKQuaternion, GLKQuaternion) -> GLKQuaternion

Returns the product of two quaternions.

func GLKQuaternionSlerp(GLKQuaternion, GLKQuaternion, Float) -> GLKQuaternion

Returns the spherical linear interpolation of two quaternions.

