

- GLKit
-  GLKVector3AllGreaterThanOrEqualToScalar(\_:\_:) 

Function

# GLKVector3AllGreaterThanOrEqualToScalar(\_:\_:)

Returns a Boolean value that states whether all the components of the source vector are greater than or equal to a scalar value.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKVector3AllGreaterThanOrEqualToScalar(
    _ vector: GLKVector3,
    _ value: Float
) -> Bool
```

## Parameters 

`vector`  

A vector.

`value`  

A scalar.

## Return Value

true if all of the vector’s components are greater than or equal to the scalar value, false otherwise.

## See Also

### Comparison Operations

func GLKVector3AllEqualToScalar(GLKVector3, Float) -> Bool

Returns a Boolean value that states whether all the components of the source vector are equal to a scalar value.

func GLKVector3AllEqualToVector3(GLKVector3, GLKVector3) -> Bool

Returns a Boolean value that indicates whether each component of the first vector is equal to the corresponding component of a second vector.

func GLKVector3AllGreaterThanOrEqualToVector3(GLKVector3, GLKVector3) -> Bool

Returns a Boolean value that indicates whether each component of the first vector is greater than or equal to the corresponding component of a second vector.

func GLKVector3AllGreaterThanScalar(GLKVector3, Float) -> Bool

Returns a Boolean value that states whether all the components of the source vector are greater than a scalar value.

func GLKVector3AllGreaterThanVector3(GLKVector3, GLKVector3) -> Bool

Returns a Boolean value that indicates whether each component of the first vector is greater than the corresponding component of a second vector.

