

- GLKit
-  GLKMatrix3MultiplyVector3(\_:\_:) 

Function

# GLKMatrix3MultiplyVector3(\_:\_:)

Multiplies a `3x3` matrix by a vector.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKMatrix3MultiplyVector3(
    _ matrixLeft: GLKMatrix3,
    _ vectorRight: GLKVector3
) -> GLKVector3
```

## Parameters 

`matrixLeft`  

The matrix multiplicand.

`vectorRight`  

The vector multiplier.

## Return Value

A new vector created by multiplying the matrix by the vector.

## See Also

### Performing Mathematical Operations on Vectors

func GLKMatrix3MultiplyVector3Array(GLKMatrix3, UnsafeMutablePointer&lt;GLKVector3>, Int)

Multiplies a `3x3` matrix by an array of vectors.

