

- UIKit
- UIViewControllerTransitioningDelegate
-  interactionControllerForPresentation(using:) 

Instance Method

# interactionControllerForPresentation(using:)

Asks your delegate for the interactive animator object to use when presenting a view controller.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
optional func interactionControllerForPresentation(using animator: any UIViewControllerAnimatedTransitioning) -> (any UIViewControllerInteractiveTransitioning)?
```

## Parameters 

`animator`  

The transition animator object returned by your animationController(forPresented:presenting:source:) method.

## Return Value

The interactive animator object to use to manage the timing of the transition or `nil` if you do not want to support interactive transitions.

## Discussion

Use this method to create and return an object that implements the methods of the UIViewControllerInteractiveTransitioning protocol. The implementation of that protocol should configure the event-handling code required to manage the appearance of the target view controller. You may return `nil` from this method if you do not want to the animations to be interactive.

Important

If you implement this method, you must also implement the animationController(forPresented:presenting:source:) method and use it to return a custom transition animator object. If the animationController(forPresented:presenting:source:) method returns `nil`, UIKit does not call this method.

For more information on implementing an interactive animator object, see UIViewControllerInteractiveTransitioning.

## See Also

### Getting the interactive animator objects

func interactionControllerForDismissal(using: any UIViewControllerAnimatedTransitioning) -> (any UIViewControllerInteractiveTransitioning)?

Asks your delegate for the interactive animator object to use when dismissing a view controller.

