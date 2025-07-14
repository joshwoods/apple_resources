

- MapKit
- MKLocalPointsOfInterestRequest
-  init(center:radius:) 

Initializer

# init(center:radius:)

Creates a points of interest search request centered on the provided coordinate with the provided radius.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
init(
    center coordinate: CLLocationCoordinate2D,
    radius: CLLocationDistance
)
```

## Parameters 

`coordinate`  

The center point of a circular region to search.

`radius`  

The radius of the region to search in meters.

## See Also

### Creating a point of interest request

init(coordinateRegion: MKCoordinateRegion)

Creates a points of interest search request based on existing region.

