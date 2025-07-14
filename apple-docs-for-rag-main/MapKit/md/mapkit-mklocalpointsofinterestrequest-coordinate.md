

- MapKit
- MKLocalPointsOfInterestRequest
-  coordinate 

Instance Property

# coordinate

The center of the point of request as latitude and longitude.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var coordinate: CLLocationCoordinate2D { get }
```

## See Also

### Configuring the request parameters

var region: MKCoordinateRegion

The region of the bounding box of the request provided or the derived bounding box of the circle created by the radius.

var radius: CLLocationDistance

The distance provided in meters or the longest distance derived from the center point to the region’s bounding box.

var pointOfInterestFilter: MKPointOfInterestFilter?

A filter that lists points of interest categories to include or exclude.

