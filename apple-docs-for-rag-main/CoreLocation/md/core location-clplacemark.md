

- Core Location
-  CLPlacemark 

Class

# CLPlacemark

A user-friendly description of a geographic coordinate, often containing the name of the place, its address, and other relevant information.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class CLPlacemark
```

## Mentioned in 

Converting between coordinates and user-friendly place names

Converting a user’s location to a descriptive placemark

## Overview

A `CLPlacemark` object stores placemark data for a given latitude and longitude. Placemark data includes information such as the country or region, state, city, and street address associated with the specified coordinate. It can also include points of interest and geographically related data.

When you reverse geocode a geographic coordinate using a CLGeocoder object, you receive a CLPlacemark object containing the descriptive information for that location. You can also create CLPlacemark object and fill it with address information yourself, which you might do when you want to determine the geographic coordinate associated with the location.

## Topics

### Creating a placemark object

init(placemark: CLPlacemark)

Initializes and returns a placemark object from another placemark object.

### Getting the placemark’s location

var location: CLLocation?

The location object containing latitude and longitude information.

var region: CLRegion?

The geographic region associated with the placemark.

### Getting the placemark name

var name: String?

The name of the placemark.

### Getting the placemark details

var thoroughfare: String?

The street address associated with the placemark.

var subThoroughfare: String?

Additional street-level information for the placemark.

var locality: String?

The city associated with the placemark.

var subLocality: String?

Additional city-level information for the placemark.

var administrativeArea: String?

The state or province associated with the placemark.

var subAdministrativeArea: String?

Additional administrative area information for the placemark.

var postalCode: String?

The postal code associated with the placemark.

### Getting the placemark’s country

var isoCountryCode: String?

The abbreviated country or region name.

var country: String?

The name of the country or region associated with the placemark.

### Getting the associated contact details

var postalAddress: CNPostalAddress?

The postal address associated with the location, formatted for use with the Contacts framework.

var addressDictionary: [AnyHashable : Any]?

A dictionary containing the Address Book keys and values for the placemark.

Deprecated

### Getting landscape information

var inlandWater: String?

The name of the inland water body associated with the placemark.

var ocean: String?

The name of the ocean associated with the placemark.

### Getting points of interest

var areasOfInterest: [String]?

The relevant areas of interest associated with the placemark.

### Getting the placemark’s time zone

var timeZone: TimeZone?

The time zone associated with the placemark.

### Type Aliases

typealias Specification

typealias UnwrappedType

typealias ValueType

### Instance Properties

var displayRepresentation: DisplayRepresentation

### Type Properties

static var defaultResolverSpecification: EmptyResolverSpecification&lt;CLPlacemark>

static var typeDisplayRepresentation: TypeDisplayRepresentation

### Initializers

convenience init(location: CLLocation, name: String?, postalAddress: CNPostalAddress?)

### Default Implementations

InstanceDisplayRepresentable Implementations

TypeDisplayRepresentable Implementations

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomLocalizedStringResourceConvertible
- CustomStringConvertible
- DisplayRepresentable
- Equatable
- Hashable
- InstanceDisplayRepresentable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable
- TypeDisplayRepresentable

## See Also

### Geocoding

Converting between coordinates and user-friendly place names

Convert between a latitude and longitude pair and a more user-friendly description of that location.

Converting a user’s location to a descriptive placemark

Transform the user’s location that displays on a map into an informative textual description by reverse geocoding.

class CLGeocoder

An interface for converting between geographic coordinates and place names.

