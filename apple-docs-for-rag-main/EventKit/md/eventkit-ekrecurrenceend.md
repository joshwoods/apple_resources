

- EventKit
-  EKRecurrenceEnd 

Class

# EKRecurrenceEnd

A class that defines the end of a recurrence rule.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
class EKRecurrenceEnd
```

## Mentioned in 

Creating a recurring event

## Overview

The `EKRecurrenceEnd` class defines the end of a recurrence rule defined by an EKRecurrenceRule object. The recurrence end can be specified by a date (date-based) or by a maximum count of occurrences (count-based). An event that is intended to continue indefinitely should have its `EKRecurrenceEnd` set to `nil`.

## Topics

### Creating a Recurrence End

convenience init(end: Date)

Initializes and returns a date-based recurrence end with a given end date.

convenience init(occurrenceCount: Int)

Initializes and returns a count-based recurrence end with a given maximum occurrence count.

### Accessing Recurrence End Properties

var endDate: Date?

The end date of the recurrence end, or `nil` if the recurrence end is count-based.

var occurrenceCount: Int

The occurrence count of the recurrence end, or `0` if the recurrence end is date-based.

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

### Recurrence

Creating a recurring event

Set up an event or reminder that repeats.

class EKRecurrenceDayOfWeek

A class that represents the day of the week.

class EKRecurrenceRule

A class that describes the pattern for a recurring event.

