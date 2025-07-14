

- GLKit
-  GLKVector4AllEqualToVector4(\_:\_:) 

Function

# GLKVector4AllEqualToVector4(\_:\_:)

Returns a Boolean value that indicates whether each component of the first vector is equal to the corresponding component of a second vector.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKVector4AllEqualToVector4(
    _ vectorLeft: GLKVector4,
    _ vectorRight: GLKVector4
) -> Bool
```

## Parameters 

`vectorLeft`  

The first vector.

`vectorRight`  

The second vector.

## Return Value

true if all of the vectors’ components are equal , false otherwise.

## See Also

### Comparison Operations

func GLKVector4AllEqualToScalar(GLKVector4, Float) -> Bool

Returns a Boolean value that states whether all the components of the source vector are equal to a scalar value.

func GLKVector4AllGreaterThanOrEqualToScalar(GLKVector4, Float) -> Bool

Returns a Boolean value that states whether all the components of the source vector are greater than or equal to a scalar value.

func GLKVector4AllGreaterThanOrEqualToVector4(GLKVector4, GLKVector4) -> Bool

Returns a Boolean value that indicates whether each component of the first vector is greater than or equal to the corresponding component of a second vector.

func GLKVector4AllGreaterThanScalar(GLKVector4, Float) -> Bool

Returns a Boolean value that states whether all the components of the source vector are greater than a scalar value.

func GLKVector4AllGreaterThanVector4(GLKVector4, GLKVector4) -> Bool

Returns a Boolean value that indicates whether each component of the first vector is greater than the corresponding component of a second vector.

