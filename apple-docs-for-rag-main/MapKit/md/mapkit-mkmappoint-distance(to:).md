

- MapKit
- MKMapPoint
-  distance(to:) 

Instance Method

# distance(to:)

Returns the number of meters between two map points.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
func distance(to b: MKMapPoint) -> CLLocationDistance
```

## Parameters 

`b`  

The second map point.

## Return Value

The number of meters between the specified map points.

## Discussion

This distance reflects the actual distance between the two points on the surface of the globe, taking into account the curvature of the Earth.

## See Also

### Getting the distance between points

func MKMetersPerMapPointAtLatitude(CLLocationDegrees) -> CLLocationDistance

Returns the distance that one map point spans at the specified latitude.

func MKMapPointsPerMeterAtLatitude(CLLocationDegrees) -> Double

Returns the number of map points that represent one meter at the specified latitude.

