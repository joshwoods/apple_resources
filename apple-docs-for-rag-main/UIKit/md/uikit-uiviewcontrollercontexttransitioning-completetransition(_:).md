

- UIKit
- UIViewControllerContextTransitioning
-  completeTransition(\_:) 

Instance Method

# completeTransition(\_:)

Notifies the system that the transition animation is done.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func completeTransition(_ didComplete: Bool)
```

**Required**

## Parameters 

`didComplete`  

true if the transition to the presented view controller completed successfully or false if the original view controller is still being displayed.

## Discussion

You must call this method after your animations have completed to notify the system that the transition animation is done. The parameter you pass must indicate whether the animations completed successfully. For interactive animations, you must call this method in addition to the finishInteractiveTransition() or cancelInteractiveTransition() method. The best place to call this method is in the completion block of your animations.

The default implementation of this method calls the animator object’s animationEnded(_:) method to give it a chance to perform any last minute cleanup.

## See Also

### Reporting the transition progress

func updateInteractiveTransition(CGFloat)

Updates the completion percentage of the transition.

**Required**

func pauseInteractiveTransition()

Tells the system to pause the animations.

**Required**

func finishInteractiveTransition()

Notifies the system that user interactions signaled the completion of the transition.

**Required**

func cancelInteractiveTransition()

Notifies the system that user interactions canceled the transition.

**Required**

var transitionWasCancelled: Bool

Returns a Boolean value indicating whether the transition was canceled.

**Required**

