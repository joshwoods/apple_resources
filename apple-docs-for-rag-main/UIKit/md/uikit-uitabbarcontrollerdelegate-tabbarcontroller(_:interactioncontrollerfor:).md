

- UIKit
- UITabBarControllerDelegate
-  tabBarController(\_:interactionControllerFor:) 

Instance Method

# tabBarController(\_:interactionControllerFor:)

Called to allow the delegate to return a UIViewControllerInteractiveTransitioning delegate object for use during an animated tab bar transition.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS

``` source
@MainActor
optional func tabBarController(
    _ tabBarController: UITabBarController,
    interactionControllerFor animationController: any UIViewControllerAnimatedTransitioning
) -> (any UIViewControllerInteractiveTransitioning)?
```

## Parameters 

`tabBarController`  

The tab bar controller participating in the interactive, animated transition.

`animationController`  

The noninteractive animation controller

## Return Value

The UIViewControllerInteractiveTransitioning delegate object responsible for managing the user interaction in an animated tab bar transition.

## See Also

### Supporting custom tab bar transition animations

func tabBarController(UITabBarController, animationControllerForTransitionFrom: UIViewController, to: UIViewController) -> (any UIViewControllerAnimatedTransitioning)?

Called to allow the delegate to return a UIViewControllerAnimatedTransitioning delegate object for use during a noninteractive tab bar view controller transition.

