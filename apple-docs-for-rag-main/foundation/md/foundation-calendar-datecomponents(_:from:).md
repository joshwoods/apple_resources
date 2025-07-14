

- Foundation
- Calendar
-  dateComponents(\_:from:) 

Instance Method

# dateComponents(\_:from:)

Returns all the date components of a date, using the calendar time zone.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func dateComponents(
    _ components: Set,
    from date: Date
) -> DateComponents
```

## Parameters 

`components`  

The components to return.

`date`  

The `Date` to use.

## Return Value

The date components of the specified date.

## Discussion

Note

If you want “date information in a given time zone” in order to display it, you should use `DateFormatter` to format the date.

## See Also

### Extracting Components

func date(Date, matchesComponents: DateComponents) -> Bool

Determines if the date has all of the specified date components.

func component(Calendar.Component, from: Date) -> Int

Returns the value for one component of a date.

func dateComponents(Set&lt;Calendar.Component>, from: Date, to: Date) -> DateComponents

Returns the difference between two dates.

func dateComponents(Set&lt;Calendar.Component>, from: DateComponents, to: DateComponents) -> DateComponents

Returns the difference between two dates specified as `DateComponents`.

func dateComponents(in: TimeZone, from: Date) -> DateComponents

Returns all the date components of a date, as if in a given time zone (instead of the `Calendar` time zone).

enum Component

An enumeration for the various components of a calendar date.

