

- SwiftUI
- AnimationTimelineSchedule
-  init(minimumInterval:paused:) 

Initializer

# init(minimumInterval:paused:)

Create a pausable schedule of dates updating at a frequency no more quickly than the provided interval.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    minimumInterval: Double? = nil,
    paused: Bool = false
)
```

## Parameters 

`minimumInterval`  

The minimum interval to update the schedule at. Pass nil to let the system pick an appropriate update interval.

`paused`  

If the schedule should stop generating updates.

