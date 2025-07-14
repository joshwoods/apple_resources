

- AppKit
- NSEvent
- NSEvent.SwipeTrackingOptions
-  lockDirection 

Type Property

# lockDirection

Clamp gestureAmount to 0 if the user starts to swipe in the opposite direction than they started.

macOS 10.7+

``` source
static var lockDirection: NSEvent.SwipeTrackingOptions { get }
```

## See Also

### Constants

static var clampGestureAmount: NSEvent.SwipeTrackingOptions

Don’t allow gestureAmount to go beyond +/-1.0

