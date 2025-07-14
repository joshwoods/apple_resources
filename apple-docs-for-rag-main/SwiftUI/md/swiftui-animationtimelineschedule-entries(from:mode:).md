

- SwiftUI
- AnimationTimelineSchedule
-  entries(from:mode:) 

Instance Method

# entries(from:mode:)

Returns entries at the frequency of the animation schedule.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func entries(
    from start: Date,
    mode: TimelineScheduleMode
) -> AnimationTimelineSchedule.Entries
```

## Discussion

When in `.lowFrequency` mode, return no entries, effectively pausing the animation.

