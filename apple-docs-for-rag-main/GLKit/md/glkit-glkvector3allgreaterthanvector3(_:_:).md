

- GLKit
-  GLKVector3AllGreaterThanVector3(\_:\_:) 

Function

# GLKVector3AllGreaterThanVector3(\_:\_:)

Returns a Boolean value that indicates whether each component of the first vector is greater than the corresponding component of a second vector.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKVector3AllGreaterThanVector3(
    _ vectorLeft: GLKVector3,
    _ vectorRight: GLKVector3
) -> Bool
```

## Parameters 

`vectorLeft`  

The first vector.

`vectorRight`  

The second vector.

## Return Value

true if each component in the first vector is greater than the corresponding component of the second vector, false otherwise.

## See Also

### Comparison Operations

func GLKVector3AllEqualToScalar(GLKVector3, Float) -> Bool

Returns a Boolean value that states whether all the components of the source vector are equal to a scalar value.

func GLKVector3AllEqualToVector3(GLKVector3, GLKVector3) -> Bool

Returns a Boolean value that indicates whether each component of the first vector is equal to the corresponding component of a second vector.

func GLKVector3AllGreaterThanOrEqualToScalar(GLKVector3, Float) -> Bool

Returns a Boolean value that states whether all the components of the source vector are greater than or equal to a scalar value.

func GLKVector3AllGreaterThanOrEqualToVector3(GLKVector3, GLKVector3) -> Bool

Returns a Boolean value that indicates whether each component of the first vector is greater than or equal to the corresponding component of a second vector.

func GLKVector3AllGreaterThanScalar(GLKVector3, Float) -> Bool

Returns a Boolean value that states whether all the components of the source vector are greater than a scalar value.

