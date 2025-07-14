

- EventKit
- EKRecurrenceEnd
-  init(end:) 

Initializer

# init(end:)

Initializes and returns a date-based recurrence end with a given end date.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
convenience init(end endDate: Date)
```

## Parameters 

`endDate`  

The end date.

## Return Value

The initialized recurrence end.

## Discussion

The end date argument must be a valid `NSDate` and not `nil`; otherwise an exception will be raised.

## See Also

### Related Documentation

Calendar and Reminders Programming Guide

### Creating a Recurrence End

convenience init(occurrenceCount: Int)

Initializes and returns a count-based recurrence end with a given maximum occurrence count.

