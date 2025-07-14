

- SwiftUI
- LongPressGesture
-  init(minimumDuration:maximumDistance:) 

Initializer

# init(minimumDuration:maximumDistance:)

Creates a long-press gesture with a minimum duration and a maximum distance that the interaction can move before the gesture fails.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
init(
    minimumDuration: Double = 0.5,
    maximumDistance: CGFloat = 10
)
```

## Parameters 

`minimumDuration`  

The minimum duration of the long press that must elapse before the gesture succeeds.

`maximumDistance`  

The maximum distance that the fingers or cursor performing the long press can move before the gesture fails.

## See Also

### Creating a long press gesture

init(minimumDuration: Double)

Creates a long-press gesture with a minimum duration

var minimumDuration: Double

The minimum duration of the long press that must elapse before the gesture succeeds.

var maximumDistance: CGFloat

The maximum distance that the long press can move before the gesture fails.

