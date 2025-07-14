

- GLKit
-  GLKVector3MultiplyScalar(\_:\_:) 

Function

# GLKVector3MultiplyScalar(\_:\_:)

Returns a new vector created by multiplying each component of a vector by a scalar value.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKVector3MultiplyScalar(
    _ vector: GLKVector3,
    _ value: Float
) -> GLKVector3
```

## Parameters 

`vector`  

A vector.

`value`  

A scalar value.

## Return Value

A new vector.

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

func GLKVector3Lerp(GLKVector3, GLKVector3, Float) -> GLKVector3

Returns a new vector created by linearly interpreting between two vectors.

func GLKVector3Project(GLKVector3, GLKVector3) -> GLKVector3

Returns a new vector created by projecting a vector onto another vector.

func GLKVector3Maximum(GLKVector3, GLKVector3) -> GLKVector3

Returns a new vector whose component value at each position is the largest component value at the same position in the source vectors.

func GLKVector3Minimum(GLKVector3, GLKVector3) -> GLKVector3

Returns a new vector whose component value at each position is the smallest component value at the same position in the source vectors.

