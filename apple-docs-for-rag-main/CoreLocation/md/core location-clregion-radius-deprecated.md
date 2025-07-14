

- Core Location
- CLRegion
-  radius Deprecated

Instance Property

# radius

The radius (measured in meters) that defines the region’s outer boundary.

macOS 10.7–10.10DeprecatedwatchOS 2.0–2.0Deprecated

``` source
var radius: CLLocationDistance { get }
```

Deprecated

Use radius in CLCircularRegion instead.

## Discussion

In iOS, use a CLCircularRegion object to manage geographic regions.

## See Also

### Deprecated

init(circularRegionWithCenter: CLLocationCoordinate2D, radius: CLLocationDistance, identifier: String)

Initializes and returns a region object defining a circular area.

Deprecated

func contains(CLLocationCoordinate2D) -> Bool

Returns a Boolean value indicating whether the region contains the specified coordinate.

Deprecated

var center: CLLocationCoordinate2D

The center point of the region.

Deprecated

