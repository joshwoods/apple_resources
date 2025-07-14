

- Foundation
-  NSDateInterval 

Class

# NSDateInterval

An object representing the span of time between a specific start date and end date.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class NSDateInterval
```

## Overview

In Swift, this object bridges to DateInterval; use NSDateInterval when you need reference semantics or other Foundation-specific behavior.

An `NSDateInterval` object represents a closed interval between two dates. The `NSDateInterval` class provides a programmatic interface for calculating the duration of a time interval and determining whether a date falls within it, as well as comparing date intervals and checking to see whether they intersect.

An `NSDateInterval` object consists of a startDate and an endDate. The startDate and endDate of a date interval can be equal, in which case its duration is `0`. However, endDate cannot occur earlier than startDate.

You can use the DateIntervalFormatter class to create string representations of `NSDateInterval` objects that are suitable for display in the current locale.

Important

The Swift overlay to the Foundation framework provides the DateInterval structure, which bridges to the `NSDateInterval` class. For more information about value types, see Working with Cocoa Frameworks in Using Swift with Cocoa and Objective-C (Swift 4.1).

## Topics

### Creating Date Intervals

convenience init()

Initializes a date interval by setting the start and end date to the current date.

init(start: Date, duration: TimeInterval)

Initializes a date interval with a given start date and duration.

convenience init(start: Date, end: Date)

Initializes a date interval from a given start date and end date.

init(coder: NSCoder)

Returns a date interval initialized from data in the given unarchiver.

### Accessing Start Date, End Date, and Duration

var startDate: Date

The start date of the date interval.

var endDate: Date

The end date of the date interval.

var duration: TimeInterval

The duration of the date interval.

### Comparing Date Intervals

func compare(DateInterval) -> ComparisonResult

Compares the receiver with the specified date interval.

func isEqual(to: DateInterval) -> Bool

Indicates whether the receiver is equal to the specified date interval.

### Determining Intersections

func intersects(DateInterval) -> Bool

Indicates whether the receiver intersects with the specified date interval.

func intersection(with: DateInterval) -> DateInterval?

Returns the intersection between the receiver and the specified date interval.

### Determining Whether a Date Occurs Within a Date Interval

func contains(Date) -> Bool

Indicates whether the receiver contains the specified date.

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

