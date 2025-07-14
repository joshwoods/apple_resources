

- PassKit (Apple Pay and Wallet)
-  PKDateComponentsRange 

Class

# PKDateComponentsRange

An object that specifies the start and end dates for a range of time.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
class PKDateComponentsRange
```

## Overview

Create a PKDateComponentsRange with date components that are valid dates and have a calendar. The PKDateComponentsRange class supports time zones in date components, and exact times are optional.

Provide a specific time and time zone in the date components to display a correct pickup time regardless of the user’s current time zone.

## Topics

### Creating a Date Range

init?(start: DateComponents, end: DateComponents)

Creates a new time range with the start and end dates and times that you specify.

### Reading the Start and End Dates

var startDateComponents: DateComponents

The start date and time of the range.

var endDateComponents: DateComponents

The end date and time of the range.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Working with shipping methods

var detail: String?

A user-readable description of the shipping method.

var dateComponentsRange: PKDateComponentsRange?

An expected range of delivery or shipping dates for a package, or the time range when an item is available for pickup.

var identifier: String?

A unique identifier for the shipping method, used by the app.

