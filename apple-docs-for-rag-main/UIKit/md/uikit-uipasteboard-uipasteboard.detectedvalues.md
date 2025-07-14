

- UIKit
- UIPasteboard
-  UIPasteboard.DetectedValues 

Structure

# UIPasteboard.DetectedValues

An object that contains common types of data that the data detection system matches for a pasteboard.

iOS 15.0+iPadOS 15.0+Mac CatalystvisionOS

``` source
struct DetectedValues
```

## Topics

### Detected patterns

var patterns: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>

A set of key paths that represent patterns that the data detection system identifies.

var probableWebSearch: String

A string that the data detection system identifies as a probable web search item.

var probableWebURL: String

A string that the data detection system identifies as a probable web URL.

### Detected values

var calendarEvents: [DDMatchCalendarEvent]

An array of calendar events that the data detection system identifies.

var emailAddresses: [DDMatchEmailAddress]

An array of email addresses that the data detection system identifies.

var flightNumbers: [DDMatchFlightNumber]

An array of flight numbers that the system data detection system identifies.

var links: [DDMatchLink]

An array of web links that the data detection system identifies.

var moneyAmounts: [DDMatchMoneyAmount]

An array of money amounts and currencies that the data detection system identifies.

var number: Double?

A number that the data detection system identifies.

var phoneNumbers: [DDMatchPhoneNumber]

An array of phone numbers that the data detection system identifies.

var postalAddresses: [DDMatchPostalAddress]

An array of postal addresses that the data detection system identifies.

var shipmentTrackingNumbers: [DDMatchShipmentTrackingNumber]

An array of parcel tracking numbers that the data detection system identifies.

## See Also

### Detecting patterns of content in pasteboard items

func detectPatterns(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, completionHandler: (Result&lt;Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, any Error>) -> ())

Requests that the data detection system identify the patterns that you specify for the pasteboard, and provide the patterns that it matches to your closure.

func detectedPatterns(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>) async throws -> Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>

Requests that the data detection system asynchronously identify the patterns that you specify for the pasteboard, and return the patterns that it matches.

func detectPatterns(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, inItemSet: IndexSet?, completionHandler: (Result&lt;[Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>], any Error>) -> ())

Requests that the data detection system identify the patterns that you specify for the pasteboard items, and provide the patterns that it matches to your closure.

func detectedPatterns(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, inItemSet: IndexSet?) async throws -> [Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>]

Requests that the data detection system asynchronously identify the patterns that you specify for the pasteboard items, and return the patterns that it matches.

func detectValues(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, completionHandler: (Result&lt;UIPasteboard.DetectedValues, any Error>) -> ())

Requests that the data detection system identify the types of data that you specify for the pasteboard, and provide the values that it matches to your closure.

func detectedValues(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>) async throws -> UIPasteboard.DetectedValues

Requests that the data detection system asynchronously identify the types of values that you specify for the pasteboard, and return the values that it matches.

func detectValues(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, inItemSet: IndexSet?, completionHandler: (Result&lt;[UIPasteboard.DetectedValues], any Error>) -> ())

Requests that the data detection system identify the types of data that you specify for the pasteboard items, and provide the values that it matches to your closure.

func detectedValues(for: Set&lt;PartialKeyPath&lt;UIPasteboard.DetectedValues>>, inItemSet: IndexSet?) async throws -> [UIPasteboard.DetectedValues]

Requests that the data detection system asynchronously identify the types of values that you specify for the pasteboard item, and return the values that it matches for each pasteboard.

struct DetectionPattern

An object that represents a pattern to detect for the pasteboard, such as a URL, text, or a number.

