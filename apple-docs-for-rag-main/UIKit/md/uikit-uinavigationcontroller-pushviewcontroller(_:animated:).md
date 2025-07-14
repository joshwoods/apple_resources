

- UIKit
- UINavigationController
-  pushViewController(\_:animated:) 

Instance Method

# pushViewController(\_:animated:)

Pushes a view controller onto the receiver’s stack and updates the display.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func pushViewController(
    _ viewController: UIViewController,
    animated: Bool
)
```

## Parameters 

`viewController`  

The view controller to push onto the stack. This object cannot be a tab bar controller. If the view controller is already on the navigation stack, this method throws an exception.

`animated`  

Specify true to animate the transition or false if you do not want the transition to be animated. You might specify false if you are setting up the navigation controller at launch time.

## Discussion

The object in the `viewController` parameter becomes the top view controller on the navigation stack. Pushing a view controller causes its view to be embedded in the navigation interface. If the `animated` parameter is true, the view is animated into position; otherwise, the view is simply displayed in its final location.

In addition to displaying the view associated with the new view controller at the top of the stack, this method also updates the navigation bar and tool bar accordingly. For information on how the navigation bar is updated, see Updating the navigation bar.

## See Also

### Pushing and popping stack items

func popViewController(animated: Bool) -> UIViewController?

Pops the top view controller from the navigation stack and updates the display.

func popToRootViewController(animated: Bool) -> [UIViewController]?

Pops all the view controllers on the stack except the root view controller and updates the display.

func popToViewController(UIViewController, animated: Bool) -> [UIViewController]?

Pops view controllers until the specified view controller is at the top of the navigation stack.

var interactivePopGestureRecognizer: UIGestureRecognizer?

The gesture recognizer responsible for popping the top view controller off the navigation stack.

