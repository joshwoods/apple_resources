

- UIKit
- UIPercentDrivenInteractiveTransition
-  finish() 

Instance Method

# finish()

Notifies the system that user interactions signaled the completion of the transition.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func finish()
```

## Discussion

This is a convenience method that calls through to the finishInteractiveTransition() method of the context object.

While tracking user interactions, your gesture recognizer or event-handling code should call this methods when the interactions suggest that the transition is now complete. For example, if the user swipes a finger, and the touch events indicate that the swipe distance crossed the threshold needed to complete the gesture, call this method when the corresponding touch events end to let the system know that it can now complete the transition.

## See Also

### Managing a transition

func update(CGFloat)

Updates the completion percentage of the transition.

func pause()

Pauses an interruptible transition animation.

func cancel()

Notifies the system that user interactions canceled the transition.

