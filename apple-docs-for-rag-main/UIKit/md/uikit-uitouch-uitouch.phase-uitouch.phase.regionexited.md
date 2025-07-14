

- UIKit
- UITouch
- UITouch.Phase
-  UITouch.Phase.regionExited 

Case

# UITouch.Phase.regionExited

A touch for a given event has left a window on the screen.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+tvOS 13.4+visionOS 1.0+

``` source
case regionExited
```

## Discussion

The UITouch.Phase.regionEntered, UITouch.Phase.regionMoved, and UITouch.Phase.regionExited phases don’t always align with the state property of a UIHoverGestureRecognizer. States of the hover gesture recognizer only apply within the context of the gesture’s view, whereas the touch states apply within the window.

## See Also

### Constants

case began

A touch for a given event has pressed down on the screen.

case moved

A touch for a given event has moved over the screen.

case stationary

A touch for a given event is pressed down on the screen, but hasn’t moved since the previous event.

case ended

A touch for a given event has lifted from the screen.

case cancelled

The system canceled tracking for a touch, for example, when the user moves the device against their face.

case regionEntered

A touch for a given event has entered a window on the screen.

case regionMoved

A touch for the given event is within a window on the screen, but has not yet pressed down.

