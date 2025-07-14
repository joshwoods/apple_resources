

- UIKit
- UIGestureRecognizer
-  delaysTouchesEnded 

Instance Property

# delaysTouchesEnded

A Boolean value that determines whether the gesture recognizer delays sending touches in an end phase to its view.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var delaysTouchesEnded: Bool { get set }
```

## Discussion

When the value of this property is true (the default) and the gesture recognizer is analyzing touch events, the window suspends delivery of touch objects in the UITouch.Phase.ended phase to the attached view. If the gesture recognizer subsequently recognizes its gesture, these touch objects are canceled (with a touchesCancelled(_:with:) message). If the gesture recognizer doesn’t recognize its gesture, the window delivers these objects in an invocation of the view’s touchesEnded(_:with:) method. Set this property to false to have touch objects in the UITouch.Phase.ended delivered to the view while the gesture recognizer is analyzing the same touches.

## See Also

### Canceling and delaying touches

var cancelsTouchesInView: Bool

A Boolean value that determines whether touches are delivered to a view when a gesture is recognized.

var delaysTouchesBegan: Bool

A Boolean value that determines whether the gesture recognizer delays sending touches in a begin phase to its view.

