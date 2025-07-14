

- Foundation
- NSDateInterval
-  init(start:duration:) 

Initializer

# init(start:duration:)

Initializes a date interval with a given start date and duration.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
init(
    start startDate: Date,
    duration: TimeInterval
)
```

## Parameters 

`startDate`  

The start date of the date interval.

`duration`  

The duration from the start date for the date interval.

Important

This method raises an `NSArgumentException` if duration is less than `0`.

## Discussion

This is the designated initializer.

## See Also

### Creating Date Intervals

convenience init()

Initializes a date interval by setting the start and end date to the current date.

convenience init(start: Date, end: Date)

Initializes a date interval from a given start date and end date.

init(coder: NSCoder)

Returns a date interval initialized from data in the given unarchiver.

