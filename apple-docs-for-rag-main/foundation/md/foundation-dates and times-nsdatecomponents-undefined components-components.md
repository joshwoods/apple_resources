

- Foundation
- Dates and Times
- NSDateComponents
-  Undefined Components 

API Collection

# Undefined Components

Constants that denote that the value of a date component is undefined.

## Overview

For example, when an NSDateComponents object is created as the result of calculating the distance in time between two dates represented by a particular calendar, the value for the weekOfYear component would be set to NSDateComponentUndefined.

## Topics

### Constants

var NSDateComponentUndefined: Int

Specifies a date component without a value.

var NSUndefinedDateComponent: Int

Specifies a date component without a value.

Deprecated

## See Also

### Validating a Date

var isValidDate: Bool

A Boolean value that indicates whether the current combination of properties represents a date which exists in the current calendar.

func isValidDate(in: Calendar) -> Bool

Returns a Boolean value that indicates whether the current combination of properties represents a date which exists in the specified calendar.

var date: Date?

The date calculated from the current components using the stored calendar.

