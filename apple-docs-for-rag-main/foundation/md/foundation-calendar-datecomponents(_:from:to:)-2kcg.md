

- Foundation
- Calendar
-  dateComponents(\_:from:to:) 

Instance Method

# dateComponents(\_:from:to:)

Returns the difference between two dates.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func dateComponents(
    _ components: Set,
    from start: Date,
    to end: Date
) -> DateComponents
```

## Parameters 

`components`  

Which components to compare.

`start`  

The starting date.

`end`  

The ending date.

## Return Value

The result of calculating the difference from start to end.

## See Also

### Extracting Components

func date(Date, matchesComponents: DateComponents) -> Bool

Determines if the date has all of the specified date components.

func component(Calendar.Component, from: Date) -> Int

Returns the value for one component of a date.

func dateComponents(Set&lt;Calendar.Component>, from: Date) -> DateComponents

Returns all the date components of a date, using the calendar time zone.

func dateComponents(Set&lt;Calendar.Component>, from: DateComponents, to: DateComponents) -> DateComponents

Returns the difference between two dates specified as `DateComponents`.

func dateComponents(in: TimeZone, from: Date) -> DateComponents

Returns all the date components of a date, as if in a given time zone (instead of the `Calendar` time zone).

enum Component

An enumeration for the various components of a calendar date.

