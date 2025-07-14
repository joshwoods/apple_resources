

- AppKit
- NSEvent
- NSEvent.SwipeTrackingOptions
-  clampGestureAmount 

Type Property

# clampGestureAmount

Don’t allow gestureAmount to go beyond +/-1.0

macOS 10.7+

``` source
static var clampGestureAmount: NSEvent.SwipeTrackingOptions { get }
```

## See Also

### Constants

static var lockDirection: NSEvent.SwipeTrackingOptions

Clamp gestureAmount to 0 if the user starts to swipe in the opposite direction than they started.

