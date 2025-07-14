

- DataDetection
-  DDMatchEmailAddress 

Class

# DDMatchEmailAddress

An object that contains an email address that the data detection system matches.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class DDMatchEmailAddress
```

## Overview

The DataDetection framework returns an email match in a `DDMatchEmailAddress` object, which includes an email address, and optionally a label that categorizes the email address.

## Topics

### Getting email information

var emailAddress: String

A string that represents an email address.

var label: String?

A string that categorizes an email address, such as Home or Work.

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

class DDMatchFlightNumber

An object that contains a flight number that the data detection system matches.

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

