

- GLKit
-  GLKVector4AllGreaterThanScalar(\_:\_:) 

Function

# GLKVector4AllGreaterThanScalar(\_:\_:)

Returns a Boolean value that states whether all the components of the source vector are greater than a scalar value.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKVector4AllGreaterThanScalar(
    _ vector: GLKVector4,
    _ value: Float
) -> Bool
```

## Parameters 

`vector`  

A vector.

`value`  

A scalar.

## Return Value

true if all of the vector’s components are greater than the scalar value, false otherwise.

## See Also

### Comparison Operations

func GLKVector4AllEqualToScalar(GLKVector4, Float) -> Bool

Returns a Boolean value that states whether all the components of the source vector are equal to a scalar value.

func GLKVector4AllEqualToVector4(GLKVector4, GLKVector4) -> Bool

Returns a Boolean value that indicates whether each component of the first vector is equal to the corresponding component of a second vector.

func GLKVector4AllGreaterThanOrEqualToScalar(GLKVector4, Float) -> Bool

Returns a Boolean value that states whether all the components of the source vector are greater than or equal to a scalar value.

func GLKVector4AllGreaterThanOrEqualToVector4(GLKVector4, GLKVector4) -> Bool

Returns a Boolean value that indicates whether each component of the first vector is greater than or equal to the corresponding component of a second vector.

func GLKVector4AllGreaterThanVector4(GLKVector4, GLKVector4) -> Bool

Returns a Boolean value that indicates whether each component of the first vector is greater than the corresponding component of a second vector.

