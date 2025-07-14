

- MapKit
- MKMapItem
-  timeZone 

Instance Property

# timeZone

The time zone of the specified location.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var timeZone: TimeZone? { get set }
```

## Discussion

When you search for map items, MapKit populates this field with the time zone information as a convenience. You may also set the time zone for any map items you create.

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

var pointOfInterestCategory: MKPointOfInterestCategory?

The point-of-interest category for the map item.

var phoneNumber: String?

The phone number associated with a business at the specified location.

var url: URL?

The URL associated with the specified location.

