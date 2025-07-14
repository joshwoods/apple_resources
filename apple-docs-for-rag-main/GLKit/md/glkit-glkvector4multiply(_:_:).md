

- GLKit
-  GLKVector4Multiply(\_:\_:) 

Function

# GLKVector4Multiply(\_:\_:)

Returns the product of two vectors.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKVector4Multiply(
    _ vectorLeft: GLKVector4,
    _ vectorRight: GLKVector4
) -> GLKVector4
```

## Parameters 

`vectorLeft`  

The first vector.

`vectorRight`  

The second vector.

## Return Value

A new vector whose components each represent the product of the components found in the same positions of the two source vectors.

## See Also

### Mathematical Operations Performed on Vectors

func GLKVector4Negate(GLKVector4) -> GLKVector4

Returns a new vector created by negating the component values of another vector.

func GLKVector4Normalize(GLKVector4) -> GLKVector4

Returns a new vector created by normalizing an input vector to a length of `1.0`.

func GLKVector4AddScalar(GLKVector4, Float) -> GLKVector4

Returns a new vector created by adding a scalar value to each component of a vector.

func GLKVector4SubtractScalar(GLKVector4, Float) -> GLKVector4

Returns a new vector created by subtracting a scalar value from each component of a vector.

func GLKVector4MultiplyScalar(GLKVector4, Float) -> GLKVector4

Returns a new vector created by multiplying each component of a vector by a scalar value.

func GLKVector4DivideScalar(GLKVector4, Float) -> GLKVector4

Returns a new vector created by dividing each component of a vector by a scalar value.

func GLKVector4Add(GLKVector4, GLKVector4) -> GLKVector4

Returns the sum of two vectors.

func GLKVector4Subtract(GLKVector4, GLKVector4) -> GLKVector4

Returns the difference between two vectors.

func GLKVector4Divide(GLKVector4, GLKVector4) -> GLKVector4

Returns a new vector created by dividing one vector by another.

func GLKVector4DotProduct(GLKVector4, GLKVector4) -> Float

Returns the dot product of two vectors.

func GLKVector4CrossProduct(GLKVector4, GLKVector4) -> GLKVector4

Returns the cross product of two vectors.

func GLKVector4Lerp(GLKVector4, GLKVector4, Float) -> GLKVector4

Returns a new vector created by linearly interpreting between two vectors.

func GLKVector4Project(GLKVector4, GLKVector4) -> GLKVector4

Returns a new vector created by projecting a vector onto another vector.

func GLKVector4Maximum(GLKVector4, GLKVector4) -> GLKVector4

Returns a new vector whose component value at each position is the largest component value at the same position in the source vectors.

func GLKVector4Minimum(GLKVector4, GLKVector4) -> GLKVector4

Returns a new vector whose component value at each position is the smallest component value at the same position in the source vectors.

