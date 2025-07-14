

- GLKit
-  GLKVector2AllGreaterThanOrEqualToVector2(\_:\_:) 

Function

# GLKVector2AllGreaterThanOrEqualToVector2(\_:\_:)

Returns a Boolean value that indicates whether each component of the first vector is greater than or equal to the corresponding component of a second vector.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKVector2AllGreaterThanOrEqualToVector2(
    _ vectorLeft: GLKVector2,
    _ vectorRight: GLKVector2
) -> Bool
```

## Parameters 

`vectorLeft`  

The first vector.

`vectorRight`  

The second vector.

## Return Value

true if each component in the first vector is greater than or equal to the corresponding component of the second vector, false otherwise.

## See Also

### Comparison Operations

func GLKVector2AllEqualToScalar(GLKVector2, Float) -> Bool

Returns a Boolean value that states whether all the components of the source vector are equal to a scalar value.

func GLKVector2AllEqualToVector2(GLKVector2, GLKVector2) -> Bool

Returns a Boolean value that indicates whether each component of the first vector is equal to the corresponding component of a second vector.

func GLKVector2AllGreaterThanOrEqualToScalar(GLKVector2, Float) -> Bool

Returns a Boolean value that states whether all the components of the source vector are greater than or equal to a scalar value.

func GLKVector2AllGreaterThanScalar(GLKVector2, Float) -> Bool

Returns a Boolean value that states whether all the components of the source vector are greater than a scalar value.

func GLKVector2AllGreaterThanVector2(GLKVector2, GLKVector2) -> Bool

Returns a Boolean value that indicates whether each component of the first vector is greater than the corresponding component of a second vector.

