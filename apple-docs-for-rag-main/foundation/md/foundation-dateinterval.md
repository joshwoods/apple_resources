

- Foundation
-  DateInterval 

Structure

# DateInterval

The span of time between a specific start date and end date.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
struct DateInterval
```

## Overview

DateInterval represents a closed date interval in the form of \[startDate, endDate\]. It is possible for the start and end dates to be the same with a duration of 0. DateInterval does not support reverse intervals i.e. intervals where the duration is less than 0 and the end date occurs earlier in time than the start date.

## Topics

### Creating a Date Interval

init()

Initializes an interval with start and end dates set to the current date and the duration set to `0`.

init(start: Date, duration: TimeInterval)

Initializes an interval with the specified start date and duration.

init(start: Date, end: Date)

Initializes an interval with the specified start and end date.

### Accessing Start Date, End Date, and Duration

var start: Date

The start date.

var end: Date

The end date.

var duration: TimeInterval

The duration.

### Determining Intersections

func intersection(with: DateInterval) -> DateInterval?

Returns an interval that represents the interval where the given date interval and the current instance intersect.

func intersects(DateInterval) -> Bool

Indicates whether this interval intersects the specified interval.

### Determining Whether a Date Occurs Within a Date Interval

func contains(Date) -> Bool

Indicates whether this interval contains the given date.

### Using Reference Types

class NSDateInterval

An object representing the span of time between a specific start date and end date.

### Instance Methods

func compare(DateInterval) -> ComparisonResult

Compares two intervals.

## Relationships

### Conforms To

- Comparable
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

### Date Representations

struct Date

A specific point in time, independent of any calendar or time zone.

typealias TimeInterval

A number of seconds.

