

- UIKit
- UIViewControllerTransitioningDelegate
-  animationController(forDismissed:) 

Instance Method

# animationController(forDismissed:)

Asks your delegate for the transition animator object to use when dismissing a view controller.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func animationController(forDismissed dismissed: UIViewController) -> (any UIViewControllerAnimatedTransitioning)?
```

## Parameters 

`dismissed`  

The view controller object that is about to be dismissed.

## Return Value

The animator object to use when dismissing the view controller or `nil` if you do not want to dismiss the view controller using a custom transition. The object you return should be capable of performing a fixed-length animation that is not interactive.

## Discussion

Use this method to create and return an object that implements the methods of the UIViewControllerAnimatedTransitioning protocol. Your implementation of that protocol must animate the disappearance of the `dismissed` view controller’s view from the screen. Use the `dismissed` parameter to initialize your object or perform any tasks necessary to prepare the transition animations. You may return `nil` from this method if you do not want to implement a custom transition animation when dismissing view controllers.

Note

You must implement this method if you also plan to use an interactive animator object to manage the disappearance of the view controller. The animator object returned by this method is responsible for executing the animations. The interactive animator object manages only the timing of the animation, not the animations themselves.

For more information on implementing a transition animator object, see UIViewControllerAnimatedTransitioning.

## See Also

### Getting the transition animator objects

func animationController(forPresented: UIViewController, presenting: UIViewController, source: UIViewController) -> (any UIViewControllerAnimatedTransitioning)?

Asks your delegate for the transition animator object to use when presenting a view controller.

