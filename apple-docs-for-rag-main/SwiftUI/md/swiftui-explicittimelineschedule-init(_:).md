

- SwiftUI
- ExplicitTimelineSchedule
-  init(\_:) 

Initializer

# init(\_:)

Creates a schedule composed of an explicit sequence of dates.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(_ dates: Entries)
```

## Parameters 

`dates`  

The sequence of dates at which a timeline view updates. Use a monotonically increasing sequence of dates, and ensure that at least one is in the future.

## Discussion

Use the entries(from:mode:) method to get the sequence of dates.

