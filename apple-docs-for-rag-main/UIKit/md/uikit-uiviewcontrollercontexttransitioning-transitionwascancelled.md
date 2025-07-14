

- UIKit
- UIViewControllerContextTransitioning
-  transitionWasCancelled 

Instance Property

# transitionWasCancelled

Returns a Boolean value indicating whether the transition was canceled.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var transitionWasCancelled: Bool { get }
```

**Required**

## Return Value

true if the transition was canceled or false if it is ongoing or finished normally.

## Discussion

You can call this method from your animator object to determine whether the transition has been canceled. Calling the cancelInteractiveTransition() method causes this method to return true.

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

func cancelInteractiveTransition()

Notifies the system that user interactions canceled the transition.

**Required**

