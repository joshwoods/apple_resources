

- UIKit
- UIViewControllerInteractiveTransitioning
-  startInteractiveTransition(\_:) 

Instance Method

# startInteractiveTransition(\_:)

Called when the system needs to set up the interactive portions of a view controller transition and start the animations.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func startInteractiveTransition(_ transitionContext: any UIViewControllerContextTransitioning)
```

**Required**

## Parameters 

`transitionContext`  

The context object containing information about the transition.

## Discussion

Your implementation of this method should use the data in the `transitionContext` parameter to configure user interactivity for the transition and then start the animations. While tracking user interactions, your event handling code should regularly call the context object’s updateInteractiveTransition(_:) method to report on how much of the transition is now complete. If events indicate that the user has canceled the transition, call the cancelInteractiveTransition() method. If events indicate that the transition has finished, call the finishInteractiveTransition() method.

## See Also

### Starting an interactive transition

var wantsInteractiveStart: Bool

A Boolean value indicating whether the transition is interactive when it starts.

