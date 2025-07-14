

- Foundation
- Calendar
-  date(from:) 

Instance Method

# date(from:)

Returns a date created from the specified components.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func date(from components: DateComponents) -> Date?
```

## Parameters 

`components`  

Used as input to the search algorithm for finding a corresponding date.

## Return Value

A new `Date`, or nil if a date could not be found which matches the components.

## See Also

### Calculating Dates from Components

func date(byAdding: DateComponents, to: Date, wrappingComponents: Bool) -> Date?

Returns a new `Date` representing the date calculated by adding components to a given date.

func date(byAdding: Calendar.Component, value: Int, to: Date, wrappingComponents: Bool) -> Date?

Returns a new `Date` representing the date calculated by adding an amount of a specific component to a given date.

func date(bySetting: Calendar.Component, value: Int, of: Date) -> Date?

Returns a new `Date` representing the date calculated by setting a specific component to a given time, and trying to keep lower components the same. If the component already has that value, this may result in a date which is the same as the given date.

func date(bySettingHour: Int, minute: Int, second: Int, of: Date, matchingPolicy: Calendar.MatchingPolicy, repeatedTimePolicy: Calendar.RepeatedTimePolicy, direction: Calendar.SearchDirection) -> Date?

Returns a new `Date` representing the date calculated by setting hour, minute, and second to a given time on a specified `Date`.

