

- SceneKit
-  SCNVector3EqualToVector3(\_:\_:) 

Function

# SCNVector3EqualToVector3(\_:\_:)

Returns a Boolean value that indicates whether the corresponding components of two vectors are equal.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func SCNVector3EqualToVector3(
    _ a: SCNVector3,
    _ b: SCNVector3
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

