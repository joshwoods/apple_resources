

- DataDetection
-  DDMatchPostalAddress 

Class

# DDMatchPostalAddress

An object that contains a postal address that the data detection system matches.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class DDMatchPostalAddress
```

## Overview

The DataDetection framework returns a postal address match in a `DDMatchPostalAddress` object, which optionally contains the matching parts of a postal address: street, city, state, postal code, and country.

## Topics

### Getting postal address information

var street: String?

The street name in a postal address.

var city: String?

The city name in a postal address.

var state: String?

The state name in a postal address.

var postalCode: String?

The postal code in a postal address.

var country: String?

The country or region name in a postal address.

## Relationships

### Inherits From

- DDMatch

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Matched data types

class DDMatchCalendarEvent

An object that represents a calendar date or date range that the data detection system matches.

class DDMatchEmailAddress

An object that contains an email address that the data detection system matches.

class DDMatchFlightNumber

An object that contains a flight number that the data detection system matches.

class DDMatchLink

An object that contains a web link that the data detection system matches.

class DDMatchMoneyAmount

An object that contains an amount of money that the data detection system matches.

class DDMatchPhoneNumber

An object that contains a phone number that the data detection system matches.

class DDMatchShipmentTrackingNumber

An object that contains parcel tracking information that the data detection system matches.

