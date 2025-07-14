

- Foundation
- Calendar
-  date(byAdding:to:wrappingComponents:) 

Instance Method

# date(byAdding:to:wrappingComponents:)

Returns a new `Date` representing the date calculated by adding components to a given date.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func date(
    byAdding components: DateComponents,
    to date: Date,
    wrappingComponents: Bool = false
) -> Date?
```

## Parameters 

`components`  

A set of values to add to the date.

`date`  

The starting date.

`wrappingComponents`  

If `true`, the component should be incremented and wrap around to zero/one on overflow, and should not cause higher components to be incremented. The default value is `false`.

## Return Value

A new date, or nil if a date could not be calculated with the given input.

## See Also

### Calculating Dates from Components

func date(from: DateComponents) -> Date?

Returns a date created from the specified components.

func date(byAdding: Calendar.Component, value: Int, to: Date, wrappingComponents: Bool) -> Date?

Returns a new `Date` representing the date calculated by adding an amount of a specific component to a given date.

func date(bySetting: Calendar.Component, value: Int, of: Date) -> Date?

Returns a new `Date` representing the date calculated by setting a specific component to a given time, and trying to keep lower components the same. If the component already has that value, this may result in a date which is the same as the given date.

func date(bySettingHour: Int, minute: Int, second: Int, of: Date, matchingPolicy: Calendar.MatchingPolicy, repeatedTimePolicy: Calendar.RepeatedTimePolicy, direction: Calendar.SearchDirection) -> Date?

Returns a new `Date` representing the date calculated by setting hour, minute, and second to a given time on a specified `Date`.

