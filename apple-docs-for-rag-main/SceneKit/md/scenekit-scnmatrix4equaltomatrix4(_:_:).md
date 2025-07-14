

- SceneKit
-  SCNMatrix4EqualToMatrix4(\_:\_:) 

Function

# SCNMatrix4EqualToMatrix4(\_:\_:)

Returns a Boolean value that indicates whether the corresponding elements of two matrices are equal.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

**macOS**

``` source
func SCNMatrix4EqualToMatrix4(
    _ a: SCNMatrix4,
    _ b: SCNMatrix4
) -> Bool
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
func SCNMatrix4EqualToMatrix4(
    _ a: SCNMatrix4,
    _ b: SCNMatrix4
) -> Bool
```

## Parameters 

`a`  

The first matrix to be compared.

`b`  

The first matrix to be compared.

## Return Value

True if each element in `matA` is exactly equal to the corresponding element in `b`.

## Discussion

This function performs a numeric (not bitwise) comparison of each pair of elements.

## See Also

### Comparing Matrices

func SCNMatrix4IsIdentity(SCNMatrix4) -> Bool

Returns a Boolean value that indicates whether the specified matrix is equal to the identity matrix.

