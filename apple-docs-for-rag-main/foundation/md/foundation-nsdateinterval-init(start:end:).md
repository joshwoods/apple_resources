

- Foundation
- NSDateInterval
-  init(start:end:) 

Initializer

# init(start:end:)

Initializes a date interval from a given start date and end date.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
convenience init(
    start startDate: Date,
    end endDate: Date
)
```

## Parameters 

`startDate`  

The start date of the date interval.

`endDate`  

The end date of the date interval.

Important

This method raises an `NSArgumentException` if endDate occurs earlier than startDate.

## See Also

### Creating Date Intervals

convenience init()

Initializes a date interval by setting the start and end date to the current date.

init(start: Date, duration: TimeInterval)

Initializes a date interval with a given start date and duration.

init(coder: NSCoder)

Returns a date interval initialized from data in the given unarchiver.

