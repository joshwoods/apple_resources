

- Foundation
- Calendar
-  dateComponents(\_:from:to:) 

Instance Method

# dateComponents(\_:from:to:)

Returns the difference between two dates specified as `DateComponents`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func dateComponents(
    _ components: Set,
    from start: DateComponents,
    to end: DateComponents
) -> DateComponents
```

## Parameters 

`components`  

Which components to compare.

`start`  

The starting date components.

`end`  

The ending date components.

## Return Value

The result of calculating the difference from start to end.

## Discussion

For components which are not specified in each `DateComponents`, but required to specify an absolute date, the base value of the component is assumed. For example, for an `DateComponents` with just a `year` and a `month` specified, a `day` of 1, and an `hour`, `minute`, `second`, and `nanosecond` of 0 are assumed. Calendrical calculations with unspecified `year` or `year` value prior to the start of a calendar are not advised. For each `DateComponents`, if its `timeZone` property is set, that time zone is used for it. If the `calendar` property is set, that is used rather than the receiving calendar, and if both the `calendar` and `timeZone` are set, the `timeZone` property value overrides the time zone of the `calendar` property.

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

func dateComponents(in: TimeZone, from: Date) -> DateComponents

Returns all the date components of a date, as if in a given time zone (instead of the `Calendar` time zone).

enum Component

An enumeration for the various components of a calendar date.

