

- DataDetection
-  DDMatchPhoneNumber 

Class

# DDMatchPhoneNumber

An object that contains a phone number that the data detection system matches.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class DDMatchPhoneNumber
```

## Overview

The DataDetection framework returns a phone number match in a `DDMatchPhoneNumber` object, which contains a phone number, and optionally a label that categorizes the phone number.

## Topics

### Getting phone information

var phoneNumber: String

A string that represents a phone number.

var label: String?

A string that categorizes a phone number, such as Home or Work.

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

class DDMatchPostalAddress

An object that contains a postal address that the data detection system matches.

class DDMatchShipmentTrackingNumber

An object that contains parcel tracking information that the data detection system matches.

