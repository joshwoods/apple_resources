

- Foundation
- NSDateComponents
-  isValidDate(in:) 

Instance Method

# isValidDate(in:)

Returns a Boolean value that indicates whether the current combination of properties represents a date which exists in the specified calendar.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isValidDate(in calendar: Calendar) -> Bool
```

## Parameters 

`calendar`  

The calendar for which to use in the calculation.

## Return Value

true if the date corresponding to the receiver’s values is valid and exists in the given calendar, otherwise false.

## Discussion

If the timeZone property is set on the receiver, the time zone property value is used.

This property should not be used for NSDateComponents objects that represent relative quantities of calendar components. To find the the next or previous date that matches a particular set of date components, use the NSCalendar instance method nextDate(after:matching:value:options:) instead.

## See Also

### Validating a Date

var isValidDate: Bool

A Boolean value that indicates whether the current combination of properties represents a date which exists in the current calendar.

var date: Date?

The date calculated from the current components using the stored calendar.

Undefined Components

Constants that denote that the value of a date component is undefined.

