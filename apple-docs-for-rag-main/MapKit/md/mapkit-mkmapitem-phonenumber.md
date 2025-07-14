

- MapKit
- MKMapItem
-  phoneNumber 

Instance Property

# phoneNumber

The phone number associated with a business at the specified location.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
var phoneNumber: String? { get set }
```

## Discussion

If there’s a relevant phone number associated with the location, such as for a business at the location, use this property to specify that value.

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

var timeZone: TimeZone?

The time zone of the specified location.

var url: URL?

The URL associated with the specified location.

