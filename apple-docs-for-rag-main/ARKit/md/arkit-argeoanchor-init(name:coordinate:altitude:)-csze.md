

- ARKit
- ARGeoAnchor
-  init(name:coordinate:altitude:) 

Initializer

# init(name:coordinate:altitude:)

Initializes a named location anchor with the given coordinates and altitude.

iOS 14.0+iPadOS 14.0+

``` source
@nonobjc
convenience init(
    name: String,
    coordinate: CLLocationCoordinate2D,
    altitude: CLLocationDistance? = nil
)
```

## Parameters 

`name`  

Name of the anchor.

`coordinate`  

Lattitude and longitude of the anchor’s geographic location.

`altitude`  

Vertical distance, in meters, between this anchor and sea level.

## See Also

### Creating a Geo Anchor

convenience init(coordinate: CLLocationCoordinate2D, altitude: CLLocationDistance?)

Initializes a location anchor with the given coordinate and altitude.

init(name: String, coordinate: CLLocationCoordinate2D, altitude: CLLocationDistance)

Initializes a named location anchor with the given coordinates and altitude.

