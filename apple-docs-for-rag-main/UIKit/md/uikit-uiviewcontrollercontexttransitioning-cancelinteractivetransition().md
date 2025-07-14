

- UIKit
- UIViewControllerContextTransitioning
-  cancelInteractiveTransition() 

Instance Method

# cancelInteractiveTransition()

Notifies the system that user interactions canceled the transition.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func cancelInteractiveTransition()
```

**Required**

## Discussion

While tracking user interactions, gesture recognizers or your interactive animator object should call this method when interactions suggest that the user wants to cancel or abort the view controller transition. For example, if the user reverses the swipe direction and touch events end, suggesting that the user decided against the transition, you would call this method.

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

func finishInteractiveTransition()

Notifies the system that user interactions signaled the completion of the transition.

**Required**

var transitionWasCancelled: Bool

Returns a Boolean value indicating whether the transition was canceled.

**Required**

