

- MapKit
- MKLocalPointsOfInterestRequest
-  init(coordinateRegion:) 

Initializer

# init(coordinateRegion:)

Creates a points of interest search request based on existing region.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
init(coordinateRegion region: MKCoordinateRegion)
```

## Parameters 

`region`  

The region to search.

## See Also

### Creating a point of interest request

init(center: CLLocationCoordinate2D, radius: CLLocationDistance)

Creates a points of interest search request centered on the provided coordinate with the provided radius.

