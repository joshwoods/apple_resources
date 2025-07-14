

- UIKit
- UINavigationControllerDelegate
-  navigationController(\_:animationControllerFor:from:to:) 

Instance Method

# navigationController(\_:animationControllerFor:from:to:)

Allows the delegate to return a noninteractive animator object for use during view controller transitions.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func navigationController(
    _ navigationController: UINavigationController,
    animationControllerFor operation: UINavigationController.Operation,
    from fromVC: UIViewController,
    to toVC: UIViewController
) -> (any UIViewControllerAnimatedTransitioning)?
```

## Parameters 

`navigationController`  

The navigation controller whose navigation stack is changing.

`operation`  

The type of transition operation that is occurring. For a list of possible values, see the UINavigationController.Operation constants.

`fromVC`  

The currently visible view controller.

`toVC`  

The view controller that should be visible at the end of the transition.

## Return Value

The animator object responsible for managing the transition animations, or `nil` if you want to use the standard navigation controller transitions. The object you return must conform to the UIViewControllerAnimatedTransitioning protocol.

## Discussion

Implement this delegate method when you want to provide a custom animated transition between view controllers as they are added to or removed from the navigation stack. The object you return should be capable of configuring and performing noninteractive animations for the specified view controllers for the specified type of operation over a fixed period of time.

If you want to allow the user to perform interactive transitions, you must *also* implement the navigationController(_:interactionControllerFor:) method.

## See Also

### Supporting custom transition animations

func navigationController(UINavigationController, interactionControllerFor: any UIViewControllerAnimatedTransitioning) -> (any UIViewControllerInteractiveTransitioning)?

Allows the delegate to return an interactive animator object for use during view controller transitions.

func navigationControllerPreferredInterfaceOrientationForPresentation(UINavigationController) -> UIInterfaceOrientation

Returns the preferred orientation for presentation of the navigation controller, as determined by the delegate.

func navigationControllerSupportedInterfaceOrientations(UINavigationController) -> UIInterfaceOrientationMask

Returns the complete set of supported interface orientations for the navigation controller, as determined by the delegate.

