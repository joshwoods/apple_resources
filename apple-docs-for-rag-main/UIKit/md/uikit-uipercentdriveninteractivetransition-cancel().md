

- UIKit
- UIPercentDrivenInteractiveTransition
-  cancel() 

Instance Method

# cancel()

Notifies the system that user interactions canceled the transition.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func cancel()
```

## Discussion

This is a convenience method that calls through to the cancelInteractiveTransition() method of the context object.

While tracking user interactions, your gesture recognizer or event-handling code would call this method when interactions suggest that the user wants to cancel or abort the view controller transition. For example, if the user reverses the swipe direction and then touch events end, suggesting that the user decided against the transition, you would call this method.

## See Also

### Managing a transition

func update(CGFloat)

Updates the completion percentage of the transition.

func pause()

Pauses an interruptible transition animation.

func finish()

Notifies the system that user interactions signaled the completion of the transition.

