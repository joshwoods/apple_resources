

- UIKit
- UITabBarControllerDelegate
-  tabBarController(\_:animationControllerForTransitionFrom:to:) 

Instance Method

# tabBarController(\_:animationControllerForTransitionFrom:to:)

Called to allow the delegate to return a UIViewControllerAnimatedTransitioning delegate object for use during a noninteractive tab bar view controller transition.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS

``` source
@MainActor
optional func tabBarController(
    _ tabBarController: UITabBarController,
    animationControllerForTransitionFrom fromVC: UIViewController,
    to toVC: UIViewController
) -> (any UIViewControllerAnimatedTransitioning)?
```

## Parameters 

`tabBarController`  

The tab bar controller whose view controller is transitioning.

`fromVC`  

The currently visible view controller.

`toVC`  

The view controller intended to be visible after the transition ends.

## Return Value

The UIViewControllerAnimatedTransitioning delegate object responsible for managing the tab bar view controller transition animation.

## See Also

### Supporting custom tab bar transition animations

func tabBarController(UITabBarController, interactionControllerFor: any UIViewControllerAnimatedTransitioning) -> (any UIViewControllerInteractiveTransitioning)?

Called to allow the delegate to return a UIViewControllerInteractiveTransitioning delegate object for use during an animated tab bar transition.

