

- Core Location
- CLLocation
-  getDistanceFrom(\_:) Deprecated

Instance Method

# getDistanceFrom(\_:)

Returns the distance (measured in meters) from the current object’s location to the specified location.

macOS 10.15–10.15Deprecated

``` source
func getDistanceFrom(_ location: CLLocation) -> CLLocationDistance
```

Deprecated

Use the distance(from:) method instead.

## Parameters 

`location`  

The other location.

## Return Value

The distance (in meters) between the two locations.

## Discussion

This method measures the distance between the location in the current object and the value in the `location` parameter. The distance is calculated by tracing a line between the two points that follows the curvature of the Earth, and measuring the length of the resulting arc. The arc is a smooth curve that does not take into account altitude changes between the two locations.

## See Also

### Measuring the distance between coordinates

func distance(from: CLLocation) -> CLLocationDistance

Returns the distance (measured in meters) from the current object’s location to the specified location.

