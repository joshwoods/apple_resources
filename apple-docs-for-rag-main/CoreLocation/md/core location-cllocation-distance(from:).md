

- Core Location
- CLLocation
-  distance(from:) 

Instance Method

# distance(from:)

Returns the distance (measured in meters) from the current object’s location to the specified location.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func distance(from location: CLLocation) -> CLLocationDistance
```

## Parameters 

`location`  

The destination location.

## Return Value

The distance (in meters) between the two locations.

## Discussion

This method measures the distance between the location in the current object and the value in the `location` parameter. The distance is calculated by tracing a line between the two points that follows the curvature of the Earth, and measuring the length of the resulting arc. The arc is a smooth curve that doesn’t take into account altitude changes between the two locations.

## See Also

### Measuring the distance between coordinates

func getDistanceFrom(CLLocation) -> CLLocationDistance

Returns the distance (measured in meters) from the current object’s location to the specified location.

Deprecated

