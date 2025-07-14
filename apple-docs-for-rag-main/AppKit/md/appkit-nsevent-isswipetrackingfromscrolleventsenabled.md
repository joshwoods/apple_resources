

- AppKit
- NSEvent
-  isSwipeTrackingFromScrollEventsEnabled 

Type Property

# isSwipeTrackingFromScrollEventsEnabled

A Boolean value that indicates whether to track fluid swipe gestures using scroll events.

macOS 10.7+

``` source
class var isSwipeTrackingFromScrollEventsEnabled: Bool { get }
```

## Discussion

If your app implements its own scrolling, or one of your responder objects tracks scroll wheel messages before they reach a scroll view, make sure the value of this property is true before you call trackSwipeEvent(options:dampenAmountThresholdMin:max:usingHandler:) to handle the event. The system defines the value of this property based on user-level preferences.

If you use NSScrollView for your app’s scrolling behavior, you don’t need to check this property. Scroll views automatically account for this behavior.

## See Also

### Configuring swipe event behaviors

func trackSwipeEvent(options: NSEvent.SwipeTrackingOptions, dampenAmountThresholdMin: CGFloat, max: CGFloat, usingHandler: (CGFloat, NSEvent.Phase, Bool, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Allows tracking and user interface feedback of scroll wheel events.

struct SwipeTrackingOptions

Constants that specify swipe-tracking options.

