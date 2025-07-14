

- MapKit
-  MKMapPointsPerMeterAtLatitude(\_:) 

Function

# MKMapPointsPerMeterAtLatitude(\_:)

Returns the number of map points that represent one meter at the specified latitude.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
func MKMapPointsPerMeterAtLatitude(_ latitude: CLLocationDegrees) -> Double
```

## Parameters 

`latitude`  

The latitude for which to return the value.

## Return Value

The number of map points that span one meter.

## Discussion

The number of map points per meter increases as the latitude approaches the poles.

## See Also

### Getting the distance between points

func distance(to: MKMapPoint) -> CLLocationDistance

Returns the number of meters between two map points.

func MKMetersPerMapPointAtLatitude(CLLocationDegrees) -> CLLocationDistance

Returns the distance that one map point spans at the specified latitude.

