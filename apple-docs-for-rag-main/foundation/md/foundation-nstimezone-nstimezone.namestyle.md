

- Foundation
- NSTimeZone
-  NSTimeZone.NameStyle 

Enumeration

# NSTimeZone.NameStyle

Constants you use to specify a style when presenting time zone names.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum NameStyle
```

## Topics

### Constants

case standard

Specifies a standard name style. For example, “Central Standard Time” for Central Time.

case shortStandard

Specifies a short name style. For example, “CST” for Central Time.

case daylightSaving

Specifies a daylight saving name style. For example, “Central Daylight Time” for Central Time.

case shortDaylightSaving

Specifies a short daylight saving name style. For example, “CDT” for Central Time.

case generic

Specifies a generic name style. For example, “Central Time” for Central Time.

case shortGeneric

Specifies a generic time zone name. For example, “CT” for Central Time.

case standard

Specifies a standard name style. For example, “Central Standard Time” for Central Time.

case shortStandard

Specifies a short name style. For example, “CST” for Central Time.

case daylightSaving

Specifies a daylight saving name style. For example, “Central Daylight Time” for Central Time.

case shortDaylightSaving

Specifies a short daylight saving name style. For example, “CDT” for Central Time.

case generic

Specifies a generic name style. For example, “Central Time” for Central Time.

case shortGeneric

Specifies a generic time zone name. For example, “CT” for Central Time.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting Time Zone Information

var name: String

The geopolitical region ID that identifies the receiver.

var abbreviation: String?

The abbreviation for the receiver, such as “EDT” (Eastern Daylight Time).

func abbreviation(for: Date) -> String?

Returns the abbreviation for the receiver at a given date.

var secondsFromGMT: Int

The current difference in seconds between the receiver and Greenwich Mean Time.

func secondsFromGMT(for: Date) -> Int

Returns the difference in seconds between the receiver and Greenwich Mean Time at a given date.

var data: Data

The data that stores the information used by the receiver.

class var timeZoneDataVersion: String

Returns the time zone data version.

