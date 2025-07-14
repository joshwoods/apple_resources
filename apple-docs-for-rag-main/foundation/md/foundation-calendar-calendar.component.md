

- Foundation
- Calendar
-  Calendar.Component 

Enumeration

# Calendar.Component

An enumeration for the various components of a calendar date.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum Component
```

## Overview

You use one or more Calendar.Component values with the component(_:from:) or dateComponents(_:from:) methods to specify parts to extract from a given Date.

The following code listing shows how to use the year, month, and day components to get the corresponding units of the current Gregorian calendar date as a DateComponents instance.

```
let myCalendar = Calendar(identifier: .gregorian)
let ymd = myCalendar.dateComponents([.year, .month, .day], from: Date())
```

## Topics

### Specifying Years and Months

case era

Identifier for the era unit.

case year

Identifier for the year unit.

case yearForWeekOfYear

Identifier for the week-counting year unit.

case quarter

Identifier for the quarter of the calendar.

case month

Identifier for the month unit.

### Specifying Weeks and Days

case weekOfYear

Identifier for the week of the year unit.

case weekOfMonth

Identifier for the week of the month calendar unit.

case weekday

Identifier for the weekday unit.

case weekdayOrdinal

Identifier for the weekday ordinal unit.

case day

Identifier for the day unit.

### Specifying Hours, Minutes, and Seconds

case hour

Identifier for the hour unit.

case minute

Identifier for the minute unit.

case second

Identifier for the second unit.

case nanosecond

Identifier for the nanosecond unit.

### Specifying Calendars and Time Zones

case calendar

Identifier for the calendar unit.

case timeZone

Identifier for the time zone unit.

### Enumeration Cases

case dayOfYear

case isLeapMonth

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Extracting Components

func date(Date, matchesComponents: DateComponents) -> Bool

Determines if the date has all of the specified date components.

func component(Calendar.Component, from: Date) -> Int

Returns the value for one component of a date.

func dateComponents(Set&lt;Calendar.Component>, from: Date) -> DateComponents

Returns all the date components of a date, using the calendar time zone.

func dateComponents(Set&lt;Calendar.Component>, from: Date, to: Date) -> DateComponents

Returns the difference between two dates.

func dateComponents(Set&lt;Calendar.Component>, from: DateComponents, to: DateComponents) -> DateComponents

Returns the difference between two dates specified as `DateComponents`.

func dateComponents(in: TimeZone, from: Date) -> DateComponents

Returns all the date components of a date, as if in a given time zone (instead of the `Calendar` time zone).

