

- GLKit
-  GLKVector2AllEqualToScalar(\_:\_:) 

Function

# GLKVector2AllEqualToScalar(\_:\_:)

Returns a Boolean value that states whether all the components of the source vector are equal to a scalar value.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKVector2AllEqualToScalar(
    _ vector: GLKVector2,
    _ value: Float
) -> Bool
```

## Parameters 

`vector`  

A vector.

`value`  

A scalar.

## Return Value

true if all of the vector’s components are equal to `value`, false otherwise.

## See Also

### Comparison Operations

func GLKVector2AllEqualToVector2(GLKVector2, GLKVector2) -> Bool

Returns a Boolean value that indicates whether each component of the first vector is equal to the corresponding component of a second vector.

func GLKVector2AllGreaterThanOrEqualToScalar(GLKVector2, Float) -> Bool

Returns a Boolean value that states whether all the components of the source vector are greater than or equal to a scalar value.

func GLKVector2AllGreaterThanOrEqualToVector2(GLKVector2, GLKVector2) -> Bool

Returns a Boolean value that indicates whether each component of the first vector is greater than or equal to the corresponding component of a second vector.

func GLKVector2AllGreaterThanScalar(GLKVector2, Float) -> Bool

Returns a Boolean value that states whether all the components of the source vector are greater than a scalar value.

func GLKVector2AllGreaterThanVector2(GLKVector2, GLKVector2) -> Bool

Returns a Boolean value that indicates whether each component of the first vector is greater than the corresponding component of a second vector.

