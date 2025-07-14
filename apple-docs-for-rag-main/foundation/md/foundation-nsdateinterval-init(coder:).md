

- Foundation
- NSDateInterval
-  init(coder:) 

Initializer

# init(coder:)

Returns a date interval initialized from data in the given unarchiver.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
init(coder: NSCoder)
```

## See Also

### Creating Date Intervals

convenience init()

Initializes a date interval by setting the start and end date to the current date.

init(start: Date, duration: TimeInterval)

Initializes a date interval with a given start date and duration.

convenience init(start: Date, end: Date)

Initializes a date interval from a given start date and end date.

