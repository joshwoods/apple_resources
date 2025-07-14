

- UIKit
- UIViewControllerTransitioningDelegate
-  interactionControllerForDismissal(using:) 

Instance Method

# interactionControllerForDismissal(using:)

Asks your delegate for the interactive animator object to use when dismissing a view controller.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
optional func interactionControllerForDismissal(using animator: any UIViewControllerAnimatedTransitioning) -> (any UIViewControllerInteractiveTransitioning)?
```

## Parameters 

`animator`  

The transition animator object returned by your animationController(forDismissed:) method.

## Return Value

The animator object that implements the code needed specifically to manage interactive transitions or `nil` if you do not want to support interactive transitions.

## Discussion

Use this method to create and return an object that implements the methods of the UIViewControllerInteractiveTransitioning protocol. The implementation of that protocol should configure the event-handling code required to manage the disappearance of the target view controller. You may return `nil` from this method if you do not want to the animations to be interactive.

Important

If you implement this method, you must also implement the animationController(forDismissed:) method and use it to return a custom transition animator object. If the animationController(forDismissed:) method returns `nil`, UIKit does not call this method.

For more information on implementing an interactive animator object, see UIViewControllerInteractiveTransitioning.

## See Also

### Getting the interactive animator objects

func interactionControllerForPresentation(using: any UIViewControllerAnimatedTransitioning) -> (any UIViewControllerInteractiveTransitioning)?

Asks your delegate for the interactive animator object to use when presenting a view controller.

