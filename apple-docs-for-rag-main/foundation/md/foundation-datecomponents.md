

- Foundation
-  DateComponents 

Structure

# DateComponents

A date or time specified in terms of units (such as year, month, day, hour, and minute) to be evaluated in a calendar system and time zone.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct DateComponents
```

## Overview

`DateComponents` encapsulates the components of a date in an extendable, structured manner.

It is used to specify a date by providing the temporal components that make up a date and time in a particular calendar: hour, minutes, seconds, day, month, year, and so on. It can also be used to specify a duration of time, for example, 5 hours and 16 minutes. A `DateComponents` is not required to define all the component fields.

When a new instance of `DateComponents` is created, the date components are set to `nil`.

## Topics

### Initializing Date Components

init(calendar: Calendar?, timeZone: TimeZone?, era: Int?, year: Int?, month: Int?, day: Int?, hour: Int?, minute: Int?, second: Int?, nanosecond: Int?, weekday: Int?, weekdayOrdinal: Int?, quarter: Int?, weekOfMonth: Int?, weekOfYear: Int?, yearForWeekOfYear: Int?)

Initializes a date components value, optionally specifying values for its fields.

var calendar: Calendar?

The calendar used to interpret the other values in this structure.

var timeZone: TimeZone?

A time zone.

### Validating a Date

var isValidDate: Bool

Indicates whether the current combination of properties represents a date which exists in the current calendar.

func isValidDate(in: Calendar) -> Bool

Indicates whether the current combination of properties represents a date which exists in the specified calendar.

var date: Date?

The date calculated from the current components using the stored calendar.

### Accessing Months and Years

var era: Int?

An era or count of eras.

var year: Int?

A year or count of years.

var yearForWeekOfYear: Int?

The year corresponding to a week-counting week.

var quarter: Int?

A quarter or count of quarters.

var month: Int?

A month or count of months.

var isLeapMonth: Bool?

Set to true if these components represent a leap month.

### Accessing Weeks and Days

var weekOfMonth: Int?

A week of the month or a count of weeks of the month.

var weekOfYear: Int?

A week of the year or count of the weeks of the year.

var weekday: Int?

A weekday or count of weekdays.

var weekdayOrdinal: Int?

A weekday ordinal or count of weekday ordinals.

var day: Int?

A day or count of days.

### Accessing Hours and Seconds

var hour: Int?

An hour or count of hours.

var minute: Int?

A minute or count of minutes.

var second: Int?

A second or count of seconds.

var nanosecond: Int?

A nanosecond or count of nanoseconds.

### Accessing Calendar Components

func value(for: Calendar.Component) -> Int?

Returns the value of one of the properties, using an enumeration value instead of a property name.

func setValue(Int?, for: Calendar.Component)

Set the value of one of the properties, using an enumeration value instead of a property name.

enum Component

An enumeration for the various components of a calendar date.

### Comparing Date Components

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Using Reference Types

class NSDateComponents

An object that specifies a date or time in terms of units (such as year, month, day, hour, and minute) to be evaluated in a calendar system and time zone.

### Initializers

init(subscriptionPeriod: Product.SubscriptionPeriod)

### Instance Properties

var dayOfYear: Int?

### Type Aliases

typealias Specification

typealias UnwrappedType

typealias ValueType

### Type Properties

static var defaultResolverSpecification: some ResolverSpecification

### Default Implementations

Equatable Implementations

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

struct Calendar

A definition of the relationships between calendar units and absolute points in time, providing features for calculation and comparison of dates.

struct TimeZone

Information about standard time conventions associated with a specific geopolitical region.

