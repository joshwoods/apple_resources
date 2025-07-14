

- UIKit
- UINavigationController
-  popToRootViewController(animated:) 

Instance Method

# popToRootViewController(animated:)

Pops all the view controllers on the stack except the root view controller and updates the display.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func popToRootViewController(animated: Bool) -> [UIViewController]?
```

## Parameters 

`animated`  

Set this value to true to animate the transition. Pass false if you are setting up a navigation controller before its view is displayed.

## Return Value

An array of view controllers representing the items that were popped from the stack.

## Discussion

The root view controller becomes the top view controller. For information on how the navigation bar is updated, see Updating the navigation bar.

## See Also

### Pushing and popping stack items

func pushViewController(UIViewController, animated: Bool)

Pushes a view controller onto the receiver’s stack and updates the display.

func popViewController(animated: Bool) -> UIViewController?

Pops the top view controller from the navigation stack and updates the display.

func popToViewController(UIViewController, animated: Bool) -> [UIViewController]?

Pops view controllers until the specified view controller is at the top of the navigation stack.

var interactivePopGestureRecognizer: UIGestureRecognizer?

The gesture recognizer responsible for popping the top view controller off the navigation stack.

