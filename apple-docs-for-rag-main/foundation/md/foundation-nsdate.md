

- Foundation
-  NSDate 

Class

# NSDate

A representation of a specific point in time, independent of any calendar or time zone.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSDate
```

## Mentioned in 

Implementing Handoff in Your App

## Overview

In Swift, use this type when you need reference semantics or other Foundation-specific behavior.

NSDate objects encapsulate a single point in time, independent of any particular calendrical system or time zone. Date objects are immutable, representing an invariant time interval relative to an absolute reference date (00:00:00 UTC on 1 January 2001).

The NSDate class provides methods for comparing dates, calculating the time interval between two dates, and creating a new date from a time interval relative to another date. NSDate objects can be used in conjunction with DateFormatter objects to create localized representations of dates and times, as well as with NSCalendar objects to perform calendar arithmetic.

NSDate is *toll-free bridged* with its Core Foundation counterpart, CFDate. See Toll-Free Bridging for more information on toll-free bridging.

Important

The Swift overlay to the Foundation framework provides the Date structure, which bridges to the NSDate class. For more information about value types, see Working with Cocoa Frameworks in Using Swift with Cocoa and Objective-C (Swift 4.1).

### Subclassing Notes

You might subclass NSDate in order to make it easier to work with a particular calendrical system, or to work with date and time values with a finer temporal granularity.

#### Methods to Override and Other Requirements

If you want to subclass NSDate to obtain behavior different than that provided by the private or public subclasses, you must:

- Declare a suitable instance variable to hold the date and time value (relative to an absolute reference date)

- Override the timeIntervalSinceReferenceDate instance method to provide the correct date and time value based on your instance variable

- Override init(timeIntervalSinceReferenceDate:), one of the designated initializer methods

- If creating a subclass that represents a calendrical system, define methods that partition past and future periods into the units of this calendar

- Implement the methods required by the NSCopying and NSCoding protocols, because NSDate adopts these protocols

#### Special Considerations

Your subclass may use a different reference date than the absolute reference date used by NSDate (00:00:00 UTC on 1 January 2001). If it does, it must still use the absolute reference date in its implementations of the methods timeIntervalSinceReferenceDate and init(timeIntervalSinceReferenceDate:). That is, the reference date referred to in the titles of these methods is the absolute reference date. If you do not use the absolute reference date in these methods, comparisons between NSDate objects of your subclass and `NSDate` objects of a private subclass will not work.

## Topics

### Creating a Date

convenience init(timeInterval: TimeInterval, sinceDate: Date)

Creates and returns a date object set to a given number of seconds from the specified date.

### Initializing a Date

init()

Returns a date object initialized to the current date and time.

convenience init(timeIntervalSinceNow: TimeInterval)

Returns a date object initialized relative to the current date and time by a given number of seconds.

convenience init(timeInterval: TimeInterval, sinceDate: Date)

Returns a date object initialized relative to another given date by a given number of seconds.

init(timeIntervalSinceReferenceDate: TimeInterval)

Returns a date object initialized relative to 00:00:00 UTC on 1 January 2001 by a given number of seconds.

convenience init(timeIntervalSince1970: TimeInterval)

Returns a date object initialized relative to 00:00:00 UTC on 1 January 1970 by a given number of seconds.

init?(coder: NSCoder)

Returns a date object initialized from data in the given unarchiver.

### Getting Temporal Boundaries

class var distantFuture: Date

A date object representing a date in the distant future.

class var distantPast: Date

A date object representing a date in the distant past.

### Retrieving the Current Date

class var now: Date

The current date and time, as of the time of access.

### Comparing Dates

func isEqual(to: Date) -> Bool

Returns a Boolean value that indicates whether a given object is a date that is exactly equal the receiver.

func earlierDate(Date) -> Date

Returns the earlier of the receiver and another given date.

func laterDate(Date) -> Date

Returns the later of the receiver and another given date.

func compare(Date) -> ComparisonResult

Indicates the temporal ordering of the receiver and another given date.

### Getting Time Intervals

func timeIntervalSince(Date) -> TimeInterval

Returns the interval between the receiver and another given date.

var timeIntervalSinceNow: TimeInterval

The interval between the date object and the current date and time.

var timeIntervalSinceReferenceDate: TimeInterval

The interval between the date object and 00:00:00 UTC on 1 January 2001.

var timeIntervalSince1970: TimeInterval

The interval between the date object and 00:00:00 UTC on 1 January 1970.

class var timeIntervalSinceReferenceDate: TimeInterval

The interval between 00:00:00 UTC on 1 January 2001 and the current date and time.

var NSTimeIntervalSince1970: Double

The number of seconds from 1 January 1970 to the reference date, 1 January 2001.

### Adding Time Intervals

func addingTimeInterval(TimeInterval) -> Self

Returns a new date object that is set to a given number of seconds relative to the receiver.

### Describing Dates

var description: String

func description(with: Any?) -> String

var customPlaygroundQuickLook: PlaygroundQuickLook

A custom playground Quick Look for this object.

Deprecated

### Recognizing Notifications

static let NSSystemClockDidChange: NSNotification.Name

A notification posted whenever the system clock is changed.

### Legacy Operations

class func date(withNaturalLanguageString: String) -> Any?

Creates and returns a date object set to the date and time specified by a given string.

Deprecated

class func date(withNaturalLanguageString: String, locale: Any?) -> Any?

Creates and returns a date object set to the date and time specified by a given string.

Deprecated

class func date(with: String) -> Any

Creates and returns a date object with a date and time value specified by a given string in the international string representation format (`YYYY-MM-DD HH:MM:SS ±HHMM`).

Deprecated

convenience init?(string: String)

Returns a date object initialized with a date and time value specified by a given string in the international string representation format.

Deprecated

func addTimeInterval(TimeInterval) -> Any

Returns a new date object that is set to a given number of seconds relative to the receiver.

Deprecated

func date(withCalendarFormat: String?, timeZone: TimeZone?) -> NSCalendarDate

Converts the receiver to a calendar date with a given format string and time zone.

Deprecated

func description(withCalendarFormat: String?, timeZone: TimeZone?, locale: Any?) -> String?Deprecated

### Initializers

convenience init(SRAbsoluteTime: SRAbsoluteTime)

convenience init(SRAbsoluteTime: SRAbsoluteTime)

### Instance Properties

var srAbsoluteTime: SRAbsoluteTime

## Relationships

### Inherits From

- NSObject

### Conforms To

- CKRecordValue
- CKRecordValueProtocol
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

