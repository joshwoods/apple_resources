

- MapKit
-  MKPlacemark 

Class

# MKPlacemark

A user-friendly description of a location on the map.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
class MKPlacemark
```

## Overview

Placemark data includes information like the country or region, state, city, and street address associated with the specified coordinate. A placemark is a concrete annotation object and conforms to the MKAnnotation protocol. Because it’s an annotation, you can add a placemark directly to the map view’s list of annotations.

## Topics

### Creating a placemark object

init(coordinate: CLLocationCoordinate2D)

Creates and returns a placemark object using the specified coordinate.

init(coordinate: CLLocationCoordinate2D, postalAddress: CNPostalAddress)

Creates and returns a placemark object with the specified coordinate and postal address from the user’s Contacts database.

init(coordinate: CLLocationCoordinate2D, addressDictionary: [String : Any]?)

Creates and returns a placemark object using the specified coordinate and Address Book dictionary.

### Accessing the placemark attributes

var countryCode: String?

The abbreviated country or region name.

## Relationships

### Inherits From

- CLPlacemark

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MKAnnotation
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Shared behavior

protocol MKAnnotation

An interface for associating your content with a specific map location.

class MKAnnotationView

The visual representation of one of your annotation objects.

