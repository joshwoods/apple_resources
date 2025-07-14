

- EventKit
- EKRecurrenceEnd
-  init(occurrenceCount:) 

Initializer

# init(occurrenceCount:)

Initializes and returns a count-based recurrence end with a given maximum occurrence count.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
convenience init(occurrenceCount: Int)
```

## Parameters 

`occurrenceCount`  

The maximum occurrence count.

## Return Value

The initialized recurrence end.

## Discussion

The maximum occurrence count argument must be a positive integer and not `0`; otherwise an exception will be raised.

## See Also

### Creating a Recurrence End

convenience init(end: Date)

Initializes and returns a date-based recurrence end with a given end date.

