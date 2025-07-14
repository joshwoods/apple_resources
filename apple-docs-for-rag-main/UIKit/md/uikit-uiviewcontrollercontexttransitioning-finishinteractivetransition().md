

- UIKit
- UIViewControllerContextTransitioning
-  finishInteractiveTransition() 

Instance Method

# finishInteractiveTransition()

Notifies the system that user interactions signaled the completion of the transition.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func finishInteractiveTransition()
```

**Required**

## Discussion

While tracking user interactions, gesture recognizers or your interactive animator object should call this method when the interactions suggest that the transition is now complete. For example, if the user swipes a finger, and the touch events indicate that the swipe distance crossed the threshold needed to complete the gesture, call this method when the corresponding touch events end to let the system know that it can now complete the transition.

Always follow calls to this method with a call to the completeTransition(_:) method to finalize the transition.

## See Also

### Reporting the transition progress

func completeTransition(Bool)

Notifies the system that the transition animation is done.

**Required**

func updateInteractiveTransition(CGFloat)

Updates the completion percentage of the transition.

**Required**

func pauseInteractiveTransition()

Tells the system to pause the animations.

**Required**

func cancelInteractiveTransition()

Notifies the system that user interactions canceled the transition.

**Required**

var transitionWasCancelled: Bool

Returns a Boolean value indicating whether the transition was canceled.

**Required**

