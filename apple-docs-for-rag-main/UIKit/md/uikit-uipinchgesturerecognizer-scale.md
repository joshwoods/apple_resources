

- UIKit
- UIPinchGestureRecognizer
-  scale 

Instance Property

# scale

The scale factor relative to the points of the two touches in screen coordinates.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var scale: CGFloat { get set }
```

## Mentioned in 

Handling pinch gestures

## Discussion

You may set the scale factor, but doing so resets the velocity.

The scale value is an absolute value that varies over time. It isn’t the delta value from the last time that the scale was reported. Apply the scale value to the state of the view when the gesture is first recognized — don’t concatenate the value each time the handler is called.

## See Also

### Interpreting the pinching gesture

var velocity: CGFloat

The velocity of the pinch in scale factor per second.

