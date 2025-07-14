

- AppKit
- NSPasteboard
-  NSPasteboard.DetectedValues 

Structure

# NSPasteboard.DetectedValues

An object that contains common types of data that the data detection system matches for a pasteboard.

macOS 15.4+

``` source
struct DetectedValues
```

## Topics

### Instance Properties

var calendarEvents: [DDMatchCalendarEvent]

An array of calendar events that the data detection system identifies.

var emailAddresses: [DDMatchEmailAddress]

An array of email addresses that the data detection system identifies.

var flightNumbers: [DDMatchFlightNumber]

An array of flight numbers that the data detection system identifies.

var links: [DDMatchLink]

An array of web links that the data detection system identifies.

var moneyAmounts: [DDMatchMoneyAmount]

An array of money amounts and currencies that the data detection system identifies.

var number: Double?

A number that the data detection system identifies.

var patterns: Set&lt;PartialKeyPath&lt;NSPasteboard.DetectedValues>>

A set of key paths that represent patterns that the data detection system identifies.

var phoneNumbers: [DDMatchPhoneNumber]

An array of phone numbers that the data detection system identifies.

var postalAddresses: [DDMatchPostalAddress]

An array of postal addresses that the data detection system identifies.

var probableWebSearch: String

A string that the data detection system identifies as a probable web search item, suitable for implementing “Paste and Search”.

var probableWebURL: String

A string that the data detection system identifies as a probable web URL, suitable for implementing “Paste and Go”.

var shipmentTrackingNumbers: [DDMatchShipmentTrackingNumber]

An array of parcel tracking numbers and carriers that the data detection system identifies.

