

- UIKit
- UIViewControllerContextTransitioning
-  pauseInteractiveTransition() 

Instance Method

# pauseInteractiveTransition()

Tells the system to pause the animations.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
func pauseInteractiveTransition()
```

**Required**

## Discussion

You can call this method in the middle of an interruptible animation to pause it.

## See Also

### Reporting the transition progress

func completeTransition(Bool)

Notifies the system that the transition animation is done.

**Required**

func updateInteractiveTransition(CGFloat)

Updates the completion percentage of the transition.

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

