

- SwiftUI
- LongPressGesture
-  minimumDuration 

Instance Property

# minimumDuration

The minimum duration of the long press that must elapse before the gesture succeeds.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
var minimumDuration: Double
```

## Mentioned in 

Adding interactivity with gestures

## See Also

### Creating a long press gesture

init(minimumDuration: Double)

Creates a long-press gesture with a minimum duration

init(minimumDuration: Double, maximumDistance: CGFloat)

Creates a long-press gesture with a minimum duration and a maximum distance that the interaction can move before the gesture fails.

var maximumDistance: CGFloat

The maximum distance that the long press can move before the gesture fails.

