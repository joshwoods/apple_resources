

- UIKit
- UINavigationControllerDelegate
-  navigationController(\_:interactionControllerFor:) 

Instance Method

# navigationController(\_:interactionControllerFor:)

Allows the delegate to return an interactive animator object for use during view controller transitions.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func navigationController(
    _ navigationController: UINavigationController,
    interactionControllerFor animationController: any UIViewControllerAnimatedTransitioning
) -> (any UIViewControllerInteractiveTransitioning)?
```

## Parameters 

`navigationController`  

The navigation controller whose navigation stack is changing.

`animationController`  

The noninteractive animator object provided by the delegate’s navigationController(_:animationControllerFor:from:to:) method.

## Return Value

The animator object responsible for managing the transition animations, or `nil` if you want to use the standard navigation controller transitions. The object you return must conform to the UIViewControllerInteractiveTransitioning protocol.

## Discussion

Implement this delegate method when you want to provide a custom, interactive transition between view controllers as they are added to or removed from the navigation stack. The object you return should configure the interactivity aspects of the transition and should work with the object in the `animationController` parameter to start the animations.

## See Also

### Supporting custom transition animations

func navigationController(UINavigationController, animationControllerFor: UINavigationController.Operation, from: UIViewController, to: UIViewController) -> (any UIViewControllerAnimatedTransitioning)?

Allows the delegate to return a noninteractive animator object for use during view controller transitions.

func navigationControllerPreferredInterfaceOrientationForPresentation(UINavigationController) -> UIInterfaceOrientation

Returns the preferred orientation for presentation of the navigation controller, as determined by the delegate.

func navigationControllerSupportedInterfaceOrientations(UINavigationController) -> UIInterfaceOrientationMask

Returns the complete set of supported interface orientations for the navigation controller, as determined by the delegate.

