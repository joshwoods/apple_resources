

- GLKit
-  GLKQuaternionRotateVector3Array(\_:\_:\_:) 

Function

# GLKQuaternionRotateVector3Array(\_:\_:\_:)

Applies a quaternion rotation to an array of vectors.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKQuaternionRotateVector3Array(
    _ quaternion: GLKQuaternion,
    _ vectors: UnsafeMutablePointer,
    _ vectorCount: Int
)
```

## Parameters 

`quaternion`  

A quaternion.

`vectors`  

On entry, an array of input vectors. On return, an array of output vectors.

`vectorCount`  

The number of vectors in the array.

## See Also

### Applying Quaternions to Vectors

func GLKQuaternionRotateVector3(GLKQuaternion, GLKVector3) -> GLKVector3

Returns a new vector that is calculated by applying a quaternion rotation to a vector.

func GLKQuaternionRotateVector4(GLKQuaternion, GLKVector4) -> GLKVector4

Returns a new vector calculated by applying a quaternion rotation to a vector.

func GLKQuaternionRotateVector4Array(GLKQuaternion, UnsafeMutablePointer&lt;GLKVector4>, Int)

Applies a quaternion rotation to an array of vectors.

