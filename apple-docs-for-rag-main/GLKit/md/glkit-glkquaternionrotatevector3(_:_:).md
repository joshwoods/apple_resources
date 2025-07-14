

- GLKit
-  GLKQuaternionRotateVector3(\_:\_:) 

Function

# GLKQuaternionRotateVector3(\_:\_:)

Returns a new vector that is calculated by applying a quaternion rotation to a vector.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKQuaternionRotateVector3(
    _ quaternion: GLKQuaternion,
    _ vector: GLKVector3
) -> GLKVector3
```

## Parameters 

`quaternion`  

A quaternion.

`vector`  

A source vector.

## Return Value

A new vector.

## See Also

### Applying Quaternions to Vectors

func GLKQuaternionRotateVector3Array(GLKQuaternion, UnsafeMutablePointer&lt;GLKVector3>, Int)

Applies a quaternion rotation to an array of vectors.

func GLKQuaternionRotateVector4(GLKQuaternion, GLKVector4) -> GLKVector4

Returns a new vector calculated by applying a quaternion rotation to a vector.

func GLKQuaternionRotateVector4Array(GLKQuaternion, UnsafeMutablePointer&lt;GLKVector4>, Int)

Applies a quaternion rotation to an array of vectors.

