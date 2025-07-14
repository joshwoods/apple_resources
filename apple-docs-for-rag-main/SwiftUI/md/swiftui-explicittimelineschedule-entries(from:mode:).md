

- SwiftUI
- ExplicitTimelineSchedule
-  entries(from:mode:) 

Instance Method

# entries(from:mode:)

Provides the sequence of dates with which you initialized the schedule.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func entries(
    from startDate: Date,
    mode: TimelineScheduleMode
) -> Entries
```

## Parameters 

`startDate`  

The date from which the sequence begins. This particular implementation of the protocol method ignores the start date.

`mode`  

The mode for the update schedule. This particular implementation of the protocol method ignores the mode.

## Return Value

The sequence of dates that you provided at initialization.

## Discussion

A TimelineView that you create with a schedule calls this TimelineSchedule method to ask the schedule when to update its content. The explicit timeline schedule implementation of this method returns the unmodified sequence of dates that you provided when you created the schedule with explicit(_:). As a result, this particular implementation ignores the `startDate` and `mode` parameters.

