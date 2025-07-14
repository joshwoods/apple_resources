

- MapKit
-  MKMapSizeEqualToSize(\_:\_:) 

Function

# MKMapSizeEqualToSize(\_:\_:)

Returns a Boolean value that indicates whether two map sizes are equal.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func MKMapSizeEqualToSize(
    _ size1: MKMapSize,
    _ size2: MKMapSize
) -> Bool
```

## Parameters 

`size1`  

The first map size.

`size2`  

The second map size.

## Return Value

true if the `width` and `height` values in both sizes are exactly the same, or false if one or both values are different.

