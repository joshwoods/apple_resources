

- GLKit
-  GLKVector3Lerp(\_:\_:\_:) 

Function

# GLKVector3Lerp(\_:\_:\_:)

Returns a new vector created by linearly interpreting between two vectors.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKVector3Lerp(
    _ vectorStart: GLKVector3,
    _ vectorEnd: GLKVector3,
    _ t: Float
) -> GLKVector3
```

## Parameters 

`vectorStart`  

The starting vector.

`vectorEnd`  

The ending vector.

`t`  

An interpolation constant.

## Return Value

A new vector.

## Discussion

The value of `t` should typically be between `0.0` and `1.0`. A value of `0.0` returns the starting vector and a value of `1.0` returns the ending vector. Any other value of `t` results in a linear interpolation between the two points.

## See Also

### Mathematical Operations Performed on Vectors

func GLKVector3Negate(GLKVector3) -> GLKVector3

Returns a new vector created by negating the component values of another vector.

func GLKVector3Normalize(GLKVector3) -> GLKVector3

Returns a new vector created by normalizing the input vector to a length of `1.0`.

func GLKVector3AddScalar(GLKVector3, Float) -> GLKVector3

Returns a new vector created by adding a scalar value to each component of a vector.

func GLKVector3SubtractScalar(GLKVector3, Float) -> GLKVector3

Returns a new vector created by subtracting a scalar value from each component of a vector.

func GLKVector3MultiplyScalar(GLKVector3, Float) -> GLKVector3

Returns a new vector created by multiplying each component of a vector by a scalar value.

func GLKVector3DivideScalar(GLKVector3, Float) -> GLKVector3

Returns a new vector created by dividing each component of a vector by a scalar value.

func GLKVector3Add(GLKVector3, GLKVector3) -> GLKVector3

Returns the sum of two vectors.

func GLKVector3Subtract(GLKVector3, GLKVector3) -> GLKVector3

Returns the difference between two vectors.

func GLKVector3Multiply(GLKVector3, GLKVector3) -> GLKVector3

Returns the product of two vectors.

func GLKVector3Divide(GLKVector3, GLKVector3) -> GLKVector3

Returns a new vector created by dividing one vector by another.

func GLKVector3DotProduct(GLKVector3, GLKVector3) -> Float

Returns the dot product of two vectors.

func GLKVector3CrossProduct(GLKVector3, GLKVector3) -> GLKVector3

Returns the cross product of two vectors.

func GLKVector3Project(GLKVector3, GLKVector3) -> GLKVector3

Returns a new vector created by projecting a vector onto another vector.

func GLKVector3Maximum(GLKVector3, GLKVector3) -> GLKVector3

Returns a new vector whose component value at each position is the largest component value at the same position in the source vectors.

func GLKVector3Minimum(GLKVector3, GLKVector3) -> GLKVector3

Returns a new vector whose component value at each position is the smallest component value at the same position in the source vectors.

