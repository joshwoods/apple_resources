

- MapKit
- MKMapItem
-  MKMapItem.Identifier 

Class

# MKMapItem.Identifier

A unique identifier for a place.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
class Identifier
```

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- RawRepresentable

## See Also

### Accessing the map item attributes

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

var timeZone: TimeZone?

The time zone of the specified location.

var url: URL?

The URL associated with the specified location.

