

- Core Location
- CLRegion
-  center Deprecated

Instance Property

# center

The center point of the region.

macOS 10.7–10.10DeprecatedwatchOS 2.0–2.0Deprecated

``` source
var center: CLLocationCoordinate2D { get }
```

Deprecated

Use center in CLCircularRegion instead.

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

var radius: CLLocationDistance

The radius (measured in meters) that defines the region’s outer boundary.

Deprecated

