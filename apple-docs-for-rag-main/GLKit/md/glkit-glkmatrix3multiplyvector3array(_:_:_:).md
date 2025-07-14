

- GLKit
-  GLKMatrix3MultiplyVector3Array(\_:\_:\_:) 

Function

# GLKMatrix3MultiplyVector3Array(\_:\_:\_:)

Multiplies a `3x3` matrix by an array of vectors.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKMatrix3MultiplyVector3Array(
    _ matrix: GLKMatrix3,
    _ vectors: UnsafeMutablePointer,
    _ vectorCount: Int
)
```

## Parameters 

`matrix`  

The matrix multiplicand.

`vectors`  

On entry, an array of input vectors. On return, an array of output vectors.

`vectorCount`  

The number of vectors in the array.

## See Also

### Performing Mathematical Operations on Vectors

func GLKMatrix3MultiplyVector3(GLKMatrix3, GLKVector3) -> GLKVector3

Multiplies a `3x3` matrix by a vector.

