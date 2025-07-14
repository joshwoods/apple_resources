

- UIKit
- UIGestureRecognizer
-  cancelsTouchesInView 

Instance Property

# cancelsTouchesInView

A Boolean value that determines whether touches are delivered to a view when a gesture is recognized.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var cancelsTouchesInView: Bool { get set }
```

## Discussion

When this property is true (the default) and the gesture recognizer recognizes its gesture, the touches of that gesture that are pending aren’t delivered to the view and previously delivered touches are canceled through a touchesCancelled(_:with:) message sent to the view. If a gesture recognizer doesn’t recognize its gesture or if the value of this property is false, the view receives all touches in the multi-touch sequence.

## See Also

### Canceling and delaying touches

var delaysTouchesBegan: Bool

A Boolean value that determines whether the gesture recognizer delays sending touches in a begin phase to its view.

var delaysTouchesEnded: Bool

A Boolean value that determines whether the gesture recognizer delays sending touches in an end phase to its view.

