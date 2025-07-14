

- Foundation
- NSDateComponents
-  isValidDate 

Instance Property

# isValidDate

A Boolean value that indicates whether the current combination of properties represents a date which exists in the current calendar.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isValidDate: Bool { get }
```

## Discussion

If the timeZone property is set on the receiver, the time zone property value is used. If the calendar property is not set on the receiver, `nil` is returned.

## See Also

### Validating a Date

func isValidDate(in: Calendar) -> Bool

Returns a Boolean value that indicates whether the current combination of properties represents a date which exists in the specified calendar.

var date: Date?

The date calculated from the current components using the stored calendar.

Undefined Components

Constants that denote that the value of a date component is undefined.

