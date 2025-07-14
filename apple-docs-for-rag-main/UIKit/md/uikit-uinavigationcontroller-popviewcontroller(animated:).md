

- UIKit
- UINavigationController
-  popViewController(animated:) 

Instance Method

# popViewController(animated:)

Pops the top view controller from the navigation stack and updates the display.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func popViewController(animated: Bool) -> UIViewController?
```

## Parameters 

`animated`  

Set this value to true to animate the transition. Pass false if you are setting up a navigation controller before its view is displayed.

## Return Value

The view controller that was popped from the stack.

## Discussion

This method removes the top view controller from the stack and makes the new top of the stack the active view controller. If the view controller at the top of the stack is the root view controller, this method does nothing. In other words, you cannot pop the last item on the stack.

In addition to displaying the view associated with the new view controller at the top of the stack, this method also updates the navigation bar and tool bar accordingly. For information on how the navigation bar is updated, see Updating the navigation bar.

## See Also

### Pushing and popping stack items

func pushViewController(UIViewController, animated: Bool)

Pushes a view controller onto the receiver’s stack and updates the display.

func popToRootViewController(animated: Bool) -> [UIViewController]?

Pops all the view controllers on the stack except the root view controller and updates the display.

func popToViewController(UIViewController, animated: Bool) -> [UIViewController]?

Pops view controllers until the specified view controller is at the top of the navigation stack.

var interactivePopGestureRecognizer: UIGestureRecognizer?

The gesture recognizer responsible for popping the top view controller off the navigation stack.

