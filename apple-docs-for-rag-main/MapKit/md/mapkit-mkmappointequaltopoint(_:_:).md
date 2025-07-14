

- MapKit
-  MKMapPointEqualToPoint(\_:\_:) 

Function

# MKMapPointEqualToPoint(\_:\_:)

Returns a Boolean value that indicates whether two map points are equal.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func MKMapPointEqualToPoint(
    _ point1: MKMapPoint,
    _ point2: MKMapPoint
) -> Bool
```

## Parameters 

`point1`  

The first map point.

`point2`  

The second point.

## Return Value

true if the `x` and `y` values in both points are exactly the same, or false if one or both values are different.

