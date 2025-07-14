

- DataDetection
-  DDMatchFlightNumber 

Class

# DDMatchFlightNumber

An object that contains a flight number that the data detection system matches.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class DDMatchFlightNumber
```

## Overview

The DataDetection framework returns a flight number match in a `DDMatchFlightNumber` object, which contains an airline name and flight number.

## Topics

### Getting flight information

var airline: String

The name of an airline.

var flightNumber: String

A string that represents a flight number.

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

class DDMatchLink

An object that contains a web link that the data detection system matches.

class DDMatchMoneyAmount

An object that contains an amount of money that the data detection system matches.

class DDMatchPhoneNumber

An object that contains a phone number that the data detection system matches.

class DDMatchPostalAddress

An object that contains a postal address that the data detection system matches.

class DDMatchShipmentTrackingNumber

An object that contains parcel tracking information that the data detection system matches.

