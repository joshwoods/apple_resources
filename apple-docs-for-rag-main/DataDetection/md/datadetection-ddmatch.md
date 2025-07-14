

- DataDetection
-  DDMatch 

Class

# DDMatch

A base class for common types of data that the data detection system matches.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class DDMatch
```

## Overview

The DataDetection framework returns results in objects that are subclasses of `DDMatch`, which are specific to the type of matching data. Each object contains the matched string.

## Topics

### Getting matches

var matchedString: String

A substring that the data detection system identifies from an original string as a common type of data.

## Relationships

### Inherits From

- NSObject

### Inherited By

- DDMatchCalendarEvent
- DDMatchEmailAddress
- DDMatchFlightNumber
- DDMatchLink
- DDMatchMoneyAmount
- DDMatchPhoneNumber
- DDMatchPostalAddress
- DDMatchShipmentTrackingNumber

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

