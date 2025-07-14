

- UIKit
- UIViewControllerContextTransitioning
-  updateInteractiveTransition(\_:) 

Instance Method

# updateInteractiveTransition(\_:)

Updates the completion percentage of the transition.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func updateInteractiveTransition(_ percentComplete: CGFloat)
```

**Required**

## Discussion

While tracking user events, gesture recognizers or your interactive animator objects should call this method regularly to update the progress toward completing the transition. If, during tracking, the interactions cross a threshold that you consider signifies the completion or cancellation of the transition, stop tracking events and call the finishInteractiveTransition() or cancelInteractiveTransition() method.

## See Also

### Reporting the transition progress

func completeTransition(Bool)

Notifies the system that the transition animation is done.

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

