

- Foundation
- Date
-  addTimeInterval(\_:) 

Instance Method

# addTimeInterval(\_:)

Adds a time interval to this date.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func addTimeInterval(_ timeInterval: TimeInterval)
```

## Parameters 

`timeInterval`  

The value to add, in seconds.

## Discussion

Warning

This only adjusts an absolute value. If you wish to add calendrical concepts like hours, days, months then you must use a `Calendar`. That will take into account complexities like daylight saving time, months with different numbers of days, and more.

## See Also

### Adding or Subtracting a Time Interval

func addingTimeInterval(TimeInterval) -> Date

Creates a new date value by adding a time interval to this date.

static func + (Date, TimeInterval) -> Date

Returns a date with a specified amount of time added to it.

static func += (inout Date, TimeInterval)

Adds a time interval to a date.

static func - (Date, TimeInterval) -> Date

Returns a `Date` with a specified amount of time subtracted from it.

static func -= (inout Date, TimeInterval)

Subtract a `TimeInterval` from a `Date`.

