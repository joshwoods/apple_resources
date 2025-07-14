

- Core Location
- CLRegion
-  init(circularRegionWithCenter:radius:identifier:) Deprecated

Initializer

# init(circularRegionWithCenter:radius:identifier:)

Initializes and returns a region object defining a circular area.

macOS 10.7–10.10DeprecatedwatchOS 2.0–2.0Deprecated

``` source
init(
    circularRegionWithCenter center: CLLocationCoordinate2D,
    radius: CLLocationDistance,
    identifier: String
)
```

Deprecated

Use init(center:radius:identifier:) in CLCircularRegion instead.

## Parameters 

`center`  

The center point of the region.

`radius`  

The distance (measured in meters) from the center point that marks the boundary of the region.

`identifier`  

A unique identifier to associate with the region object. You use this identifier to differentiate regions within your application. This value must not be `nil`.

## Return Value

An initialized region object.

## Discussion

In iOS, use a CLCircularRegion object to manage geographic regions.

## See Also

### Deprecated

func contains(CLLocationCoordinate2D) -> Bool

Returns a Boolean value indicating whether the region contains the specified coordinate.

Deprecated

var center: CLLocationCoordinate2D

The center point of the region.

Deprecated

var radius: CLLocationDistance

The radius (measured in meters) that defines the region’s outer boundary.

Deprecated

