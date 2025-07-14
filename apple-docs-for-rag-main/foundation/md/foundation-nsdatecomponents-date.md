

- Foundation
- NSDateComponents
-  date 

Instance Property

# date

The date calculated from the current components using the stored calendar.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var date: Date? { get }
```

## Discussion

Returns `nil` if the calendar property value of the receiver is `nil` or cannot convert the receiver into an NSDate object.

See Calendars, Date Components, and Calendar Units in Date and Time Programming Guide.

## See Also

### Related Documentation

Date and Time Programming Guide

### Validating a Date

var isValidDate: Bool

A Boolean value that indicates whether the current combination of properties represents a date which exists in the current calendar.

func isValidDate(in: Calendar) -> Bool

Returns a Boolean value that indicates whether the current combination of properties represents a date which exists in the specified calendar.

Undefined Components

Constants that denote that the value of a date component is undefined.

