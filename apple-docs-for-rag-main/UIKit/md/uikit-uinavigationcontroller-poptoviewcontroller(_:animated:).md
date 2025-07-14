

- UIKit
- UINavigationController
-  popToViewController(\_:animated:) 

Instance Method

# popToViewController(\_:animated:)

Pops view controllers until the specified view controller is at the top of the navigation stack.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func popToViewController(
    _ viewController: UIViewController,
    animated: Bool
) -> [UIViewController]?
```

## Parameters 

`viewController`  

The view controller that you want to be at the top of the stack. This view controller must currently be on the navigation stack.

`animated`  

Set this value to true to animate the transition. Pass false if you are setting up a navigation controller before its view is displayed.

## Return Value

An array containing the view controllers that were popped from the stack.

## Discussion

For information on how the navigation bar is updated, see Updating the navigation bar.

## See Also

### Pushing and popping stack items

func pushViewController(UIViewController, animated: Bool)

Pushes a view controller onto the receiver’s stack and updates the display.

func popViewController(animated: Bool) -> UIViewController?

Pops the top view controller from the navigation stack and updates the display.

func popToRootViewController(animated: Bool) -> [UIViewController]?

Pops all the view controllers on the stack except the root view controller and updates the display.

var interactivePopGestureRecognizer: UIGestureRecognizer?

The gesture recognizer responsible for popping the top view controller off the navigation stack.

