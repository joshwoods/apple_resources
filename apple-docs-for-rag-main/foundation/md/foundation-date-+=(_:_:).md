

- Foundation
- Date
-  +=(\_:\_:) 

Operator

# +=(\_:\_:)

Adds a time interval to a date.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func += (lhs: inout Date, rhs: TimeInterval)
```

## Parameters 

`lhs`  

A date.

`rhs`  

A TimeInterval to add to the date.

## Discussion

Warning

This only adjusts an absolute value. If you wish to add calendrical concepts like hours, days, months then you must use a `Calendar`. This takes into account complexities like daylight saving time, months with different numbers of days, and more.

## See Also

### Adding or Subtracting a Time Interval

func addTimeInterval(TimeInterval)

Adds a time interval to this date.

func addingTimeInterval(TimeInterval) -> Date

Creates a new date value by adding a time interval to this date.

static func + (Date, TimeInterval) -> Date

Returns a date with a specified amount of time added to it.

static func - (Date, TimeInterval) -> Date

Returns a `Date` with a specified amount of time subtracted from it.

static func -= (inout Date, TimeInterval)

Subtract a `TimeInterval` from a `Date`.

