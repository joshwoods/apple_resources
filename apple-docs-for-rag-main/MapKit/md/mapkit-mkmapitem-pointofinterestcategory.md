

- MapKit
- MKMapItem
-  pointOfInterestCategory 

Instance Property

# pointOfInterestCategory

The point-of-interest category for the map item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var pointOfInterestCategory: MKPointOfInterestCategory? { get set }
```

## Discussion

If the map item doesn’t correspond to a point of interest, or if the point of interest isn’t one of the known values in MKPointOfInterestCategory, pointOfInterestCategory is `nil`.

## See Also

### Accessing the map item attributes

class Identifier

A unique identifier for a place.

var alternateIdentifiers: Set&lt;MKMapItem.Identifier>

A set of alternative identifiers for a place.

var identifier: MKMapItem.Identifier?

A unique identifier for a place.

var isCurrentLocation: Bool

A Boolean value that indicates whether the map item represents the user’s location.

var name: String?

The descriptive name associated with the map item.

var placemark: MKPlacemark

The placemark object containing the location information.

var phoneNumber: String?

The phone number associated with a business at the specified location.

var timeZone: TimeZone?

The time zone of the specified location.

var url: URL?

The URL associated with the specified location.

