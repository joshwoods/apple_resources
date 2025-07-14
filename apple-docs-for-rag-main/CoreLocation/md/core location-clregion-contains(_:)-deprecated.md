

- Core Location
- CLRegion
-  contains(\_:) Deprecated

Instance Method

# contains(\_:)

Returns a Boolean value indicating whether the region contains the specified coordinate.

macOS 10.7–10.10DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func contains(_ coordinate: CLLocationCoordinate2D) -> Bool
```

Deprecated

Use contains(_:) in CLCircularRegion instead.

## Parameters 

`coordinate`  

The coordinate to test against the region.

## Return Value

true if the coordinate lies within the region’s boundaries or false if it does not.

## Discussion

In iOS, use a CLCircularRegion object to manage geographic regions.

## See Also

### Deprecated

init(circularRegionWithCenter: CLLocationCoordinate2D, radius: CLLocationDistance, identifier: String)

Initializes and returns a region object defining a circular area.

Deprecated

var center: CLLocationCoordinate2D

The center point of the region.

Deprecated

var radius: CLLocationDistance

The radius (measured in meters) that defines the region’s outer boundary.

Deprecated

