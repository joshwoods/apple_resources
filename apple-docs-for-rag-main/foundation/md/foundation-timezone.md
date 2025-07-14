

- Foundation
-  TimeZone 

Structure

# TimeZone

Information about standard time conventions associated with a specific geopolitical region.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct TimeZone
```

## Overview

`TimeZone` defines the behavior of a time zone. Time zone values represent geopolitical regions. Consequently, these values have names for these regions. Time zone values also represent a temporal offset, either plus or minus, from Greenwich Mean Time (GMT) and an abbreviation (such as PST for Pacific Standard Time).

`TimeZone` provides two static functions to get time zone values: `current` and `autoupdatingCurrent`. The `autoupdatingCurrent` time zone automatically tracks updates made by the user.

Note that time zone database entries such as “America/Los_Angeles” are IDs, not names. An example of a time zone name is “Pacific Daylight Time”. Although many `TimeZone` functions include the word “name”, they refer to IDs.

Cocoa does not provide any API to change the time zone of the computer, or of other applications.

## Topics

### Getting the Current Time Zone

static var autoupdatingCurrent: TimeZone

The time zone currently used by the system, automatically updating to the user’s current preference.

static var current: TimeZone

The time zone currently used by the system.

### Creating a Time Zone

init?(secondsFromGMT: Int)

Returns a time zone initialized with a specific number of seconds from GMT.

static var knownTimeZoneIdentifiers: [String]

Returns an array of strings listing the identifier of all the time zones known to the system.

static var abbreviationDictionary: [String : String]

Returns the mapping of abbreviations to time zone identifiers.

### Getting Time Zone Information

var identifier: String

The geopolitical region identifier that identifies the time zone.

func abbreviation(for: Date) -> String?

Returns the abbreviation for the time zone at a given date.

func secondsFromGMT(for: Date) -> Int

The current difference in seconds between the time zone and Greenwich Mean Time.

static var timeZoneDataVersion: String

Returns the time zone data version.

### Working with Daylight Savings

func isDaylightSavingTime(for: Date) -> Bool

Returns a Boolean value that indicates whether the receiver uses daylight saving time at a given date.

func daylightSavingTimeOffset(for: Date) -> TimeInterval

Returns the daylight saving time offset for a given date.

var nextDaylightSavingTimeTransition: Date?

The date of the next (after the current instant) daylight saving time transition for the time zone.

func nextDaylightSavingTimeTransition(after: Date) -> Date?

Returns the next daylight saving time transition after a given date.

### Describing Time Zones

func localizedName(for: TimeZone.NameStyle, locale: Locale?) -> String?

Returns the name of the receiver localized for a given locale.

### Using Reference Types

class NSTimeZone

Information about standard time conventions associated with a specific geopolitical region.

### Initializers

init?(abbreviation: String)

init?(identifier: String)

### Type Aliases

typealias NameStyle

### Type Properties

static var gmt: TimeZone

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- ReferenceConvertible
- Sendable

## See Also

### Calendrical Calculations

struct DateComponents

A date or time specified in terms of units (such as year, month, day, hour, and minute) to be evaluated in a calendar system and time zone.

struct Calendar

A definition of the relationships between calendar units and absolute points in time, providing features for calculation and comparison of dates.

