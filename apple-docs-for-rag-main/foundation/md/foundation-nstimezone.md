

- Foundation
-  NSTimeZone 

Class

# NSTimeZone

Information about standard time conventions associated with a specific geopolitical region.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSTimeZone
```

## Overview

In Swift, this type bridges to TimeZone; use NSTimeZone when you need reference semantics or other Foundation-specific behavior.

Time zones represent the standard time policies for a geopolitical region. Time zones have identifiers like “America/Los_Angeles” and can also be identified by abbreviations, such as PST for Pacific Standard Time. You can create time zone objects by ID with init(name:) and by abbreviation with init(abbreviation:).

Note

Time zone database entries such as “America/Los_Angeles” are IDs, not names. An example of a time zone name is “Pacific Daylight Time”. Although many NSTimeZone symbols include the word “name”, they actually refer to IDs.

Time zones can also represent a temporal offset—either plus or minus—from Greenwich Mean Time (GMT). For example, the temporal offset of Pacific Standard Time is 8 hours behind Greenwich Mean Time (GMT-8). You can create time zone objects with a temporal offset by using init(forSecondsFromGMT:).

You typically work with system time zones rather than creating time zones by identifier or by offset. The system class property returns the time zone currently used by the system, if known. This value is cached once the property is accessed and doesn’t reflect any system time zone changes until you call the resetSystemTimeZone() method. The local class property returns an autoupdating proxy object that always returns the current time zone used by the system. You can also set the default class property to make your app run as if it were in a different time zone than the system.

Tip

You can’t use NSTimeZone APIs to change the time zone of the device or of other apps.

NSTimeZone is *toll-free bridged* with its Core Foundation counterpart, CFTimeZone. See Toll-Free Bridging for more information on toll-free bridging.

Important

The Swift overlay to the Foundation framework provides the TimeZone structure, which bridges to the NSTimeZone class. For more information about value types, see Working with Cocoa Frameworks in Using Swift with Cocoa and Objective-C (Swift 4.1).

## Topics

### Working with System Time Zones

class var local: TimeZone

An object that tracks the current system time zone.

class var system: TimeZone

The time zone currently used by the system.

class func resetSystemTimeZone()

Clears any time zone value cached for the system property.

class var `default`: TimeZone

The default time zone for the current app.

### Creating Time Zones

init?(name: String)

Returns a time zone initialized with a given identifier.

init?(name: String, data: Data?)

Initializes a time zone with a given identifier and time zone data.

convenience init?(abbreviation: String)

Returns the time zone object identified by a given abbreviation.

convenience init(forSecondsFromGMT: Int)

Returns a time zone object offset from Greenwich Mean Time by a given number of seconds.

class var knownTimeZoneNames: [String]

Returns an array of strings listing the IDs of all the time zones known to the system.

class var abbreviationDictionary: [String : String]

Returns a dictionary holding the mappings of time zone abbreviations to time zone names.

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

enum NameStyle

Constants you use to specify a style when presenting time zone names.

### Working with Daylight Savings

var isDaylightSavingTime: Bool

A Boolean value that indicates whether the receiver is currently using daylight saving time.

func isDaylightSavingTime(for: Date) -> Bool

Indicates whether the receiver uses daylight saving time on a given date.

var daylightSavingTimeOffset: TimeInterval

The current daylight saving time offset of the receiver.

func daylightSavingTimeOffset(for: Date) -> TimeInterval

Returns the daylight saving time offset for a given date.

var nextDaylightSavingTimeTransition: Date?

The date of the next daylight saving time transition for the receiver.

func nextDaylightSavingTimeTransition(after: Date) -> Date?

Returns the next daylight saving time transition after a given date.

### Comparing Time Zones

func isEqual(to: TimeZone) -> Bool

Indicates whether the receiver has the same name and data as the specified time zone.

### Describing Time Zones

func localizedName(NSTimeZone.NameStyle, locale: Locale?) -> String?

Returns the localized name of the time zone.

var description: String

### Recognizing Notifications

static let NSSystemTimeZoneDidChange: NSNotification.Name

A notification posted when the time zone changes.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

