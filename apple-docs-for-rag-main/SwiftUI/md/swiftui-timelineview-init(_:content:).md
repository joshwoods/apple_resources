

- SwiftUI
- TimelineView
-  init(\_:content:) 

Initializer

# init(\_:content:)

Creates a new timeline view that uses the given schedule.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
init(
    _ schedule: Schedule,
    @ViewBuilder content: @escaping (TimelineViewDefaultContext) -> Content
)
```

Available when `Schedule` conforms to `TimelineSchedule` and `Content` conforms to `View`.

Show all declarations

## Parameters 

`schedule`  

A schedule that produces a sequence of dates that indicate the instances when the view should update. Use a type that conforms to TimelineSchedule, like everyMinute, or a custom timeline schedule that you define.

`content`  

A closure that generates view content at the moments indicated by the schedule. The closure takes an input of type TimelineViewDefaultContext that includes the date from the schedule that prompted the update, as well as a TimelineView.Context.Cadence value that the view can use to customize its appearance.

