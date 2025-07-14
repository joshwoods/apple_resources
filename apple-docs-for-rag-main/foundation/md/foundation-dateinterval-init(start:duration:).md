

- Foundation
- DateInterval
-  init(start:duration:) 

Initializer

# init(start:duration:)

Initializes an interval with the specified start date and duration.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
init(
    start: Date,
    duration: TimeInterval
)
```

## Discussion

Precondition: `duration >= 0`

## See Also

### Creating a Date Interval

init()

Initializes an interval with start and end dates set to the current date and the duration set to `0`.

init(start: Date, end: Date)

Initializes an interval with the specified start and end date.

