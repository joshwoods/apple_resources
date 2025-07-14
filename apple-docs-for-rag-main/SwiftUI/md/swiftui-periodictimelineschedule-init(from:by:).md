

- SwiftUI
- PeriodicTimelineSchedule
-  init(from:by:) 

Initializer

# init(from:by:)

Creates a periodic update schedule.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    from startDate: Date,
    by interval: TimeInterval
)
```

## Parameters 

`startDate`  

The date on which to start the sequence.

`interval`  

The time interval between successive sequence entries.

## Discussion

Use the entries(from:mode:) method to get the sequence of dates.

