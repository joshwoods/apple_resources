

- Foundation
- Date
-  +(\_:\_:) 

Operator

# +(\_:\_:)

Returns a date with a specified amount of time added to it.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func + (lhs: Date, rhs: TimeInterval) -> Date
```

## Parameters 

`lhs`  

A date.

`rhs`  

A TimeInterval to add to the date.

## Return Value

A date with a specified amount of time added to it.

## See Also

### Adding or Subtracting a Time Interval

func addTimeInterval(TimeInterval)

Adds a time interval to this date.

func addingTimeInterval(TimeInterval) -> Date

Creates a new date value by adding a time interval to this date.

static func += (inout Date, TimeInterval)

Adds a time interval to a date.

static func - (Date, TimeInterval) -> Date

Returns a `Date` with a specified amount of time subtracted from it.

static func -= (inout Date, TimeInterval)

Subtract a `TimeInterval` from a `Date`.

