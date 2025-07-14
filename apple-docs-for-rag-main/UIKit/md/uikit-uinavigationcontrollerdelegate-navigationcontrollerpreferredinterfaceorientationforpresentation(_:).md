

- UIKit
- UINavigationControllerDelegate
-  navigationControllerPreferredInterfaceOrientationForPresentation(\_:) 

Instance Method

# navigationControllerPreferredInterfaceOrientationForPresentation(\_:)

Returns the preferred orientation for presentation of the navigation controller, as determined by the delegate.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func navigationControllerPreferredInterfaceOrientationForPresentation(_ navigationController: UINavigationController) -> UIInterfaceOrientation
```

## Parameters 

`navigationController`  

The navigation controller

## Return Value

The preferred orientation for presenting the navigation controller.

## See Also

### Supporting custom transition animations

func navigationController(UINavigationController, animationControllerFor: UINavigationController.Operation, from: UIViewController, to: UIViewController) -> (any UIViewControllerAnimatedTransitioning)?

Allows the delegate to return a noninteractive animator object for use during view controller transitions.

func navigationController(UINavigationController, interactionControllerFor: any UIViewControllerAnimatedTransitioning) -> (any UIViewControllerInteractiveTransitioning)?

Allows the delegate to return an interactive animator object for use during view controller transitions.

func navigationControllerSupportedInterfaceOrientations(UINavigationController) -> UIInterfaceOrientationMask

Returns the complete set of supported interface orientations for the navigation controller, as determined by the delegate.

