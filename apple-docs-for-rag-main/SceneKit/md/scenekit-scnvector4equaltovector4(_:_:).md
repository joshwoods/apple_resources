

- SceneKit
-  SCNVector4EqualToVector4(\_:\_:) 

Function

# SCNVector4EqualToVector4(\_:\_:)

Returns a Boolean value that indicates whether the corresponding components of two vectors are equal.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func SCNVector4EqualToVector4(
    _ a: SCNVector4,
    _ b: SCNVector4
) -> Bool
```

## Parameters 

`a`  

The first vector.

`b`  

The second vector.

## Return Value

True if each component of `a` is exactly equal to `b`.

## Discussion

This function performs a numeric (not bitwise) comparison of each pair of component values.

