

- GLKit
-  GLKVector2Subtract(\_:\_:) 

Function

# GLKVector2Subtract(\_:\_:)

Returns the difference between two vectors.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKVector2Subtract(
    _ vectorLeft: GLKVector2,
    _ vectorRight: GLKVector2
) -> GLKVector2
```

## Parameters 

`vectorLeft`  

The starting vector.

`vectorRight`  

The vector to subtract.

## Return Value

A new vector whose components each represent the difference between the components found in the same positions of the two source vectors.

## See Also

### Mathematical Operations Performed on Vectors

func GLKVector2Negate(GLKVector2) -> GLKVector2

Returns a new vector created by negating the component values of another vector.

func GLKVector2Normalize(GLKVector2) -> GLKVector2

Returns a new vector created by normalizing an input vector to a length of `1.0`.

func GLKVector2AddScalar(GLKVector2, Float) -> GLKVector2

Returns a new vector created by adding a scalar value to each component of a vector.

func GLKVector2SubtractScalar(GLKVector2, Float) -> GLKVector2

Returns a new vector created by subtracting a scalar value from each component of a vector.

func GLKVector2MultiplyScalar(GLKVector2, Float) -> GLKVector2

Returns a new vector created by multiplying each component of a vector by a scalar value.

func GLKVector2DivideScalar(GLKVector2, Float) -> GLKVector2

Returns a new vector created by dividing each component of a vector by a scalar value.

func GLKVector2Add(GLKVector2, GLKVector2) -> GLKVector2

Returns the sum of two vectors.

func GLKVector2Multiply(GLKVector2, GLKVector2) -> GLKVector2

Returns a new vector created by multiplying one vector by another.

func GLKVector2Divide(GLKVector2, GLKVector2) -> GLKVector2

Returns a new vector created by dividing one vector by another.

func GLKVector2DotProduct(GLKVector2, GLKVector2) -> Float

Returns the dot product of two vectors.

func GLKVector2Lerp(GLKVector2, GLKVector2, Float) -> GLKVector2

Returns a new vector created by linearly interpreting between two vectors.

func GLKVector2Project(GLKVector2, GLKVector2) -> GLKVector2

Returns a new vector created by projecting a vector onto another vector

func GLKVector2Maximum(GLKVector2, GLKVector2) -> GLKVector2

Returns a new vector whose component value at each position is the largest component value at the same position of the two source vectors.

func GLKVector2Minimum(GLKVector2, GLKVector2) -> GLKVector2

Returns a new vector whose component value at each position is the smallest component value at the same position of the two source vectors.

