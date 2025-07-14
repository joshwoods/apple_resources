

- UIKit
- UIGestureRecognizer
-  delaysTouchesBegan 

Instance Property

# delaysTouchesBegan

A Boolean value that determines whether the gesture recognizer delays sending touches in a begin phase to its view.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var delaysTouchesBegan: Bool { get set }
```

## Discussion

When the value of this property is false (the default), views analyze touch events in UITouch.Phase.began and UITouch.Phase.moved in parallel with the gesture recognizer. When the value of the property is true, the window suspends delivery of touch objects in the UITouch.Phase.began phase to the view. If the gesture recognizer subsequently recognizes its gesture, these touch objects are discarded. If the gesture recognizer, however, doesn’t recognize its gesture, the window delivers these objects to the view in a touchesBegan(_:with:) message (and possibly a follow-up touchesMoved(_:with:) message to inform it of the touches’ current locations). Set this property to true to prevent views from processing any touches in the UITouch.Phase.began phase that may be recognized as part of this gesture.

## See Also

### Canceling and delaying touches

var cancelsTouchesInView: Bool

A Boolean value that determines whether touches are delivered to a view when a gesture is recognized.

var delaysTouchesEnded: Bool

A Boolean value that determines whether the gesture recognizer delays sending touches in an end phase to its view.

