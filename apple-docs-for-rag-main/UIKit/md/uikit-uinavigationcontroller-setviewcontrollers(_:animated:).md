

- UIKit
- UINavigationController
-  setViewControllers(\_:animated:) 

Instance Method

# setViewControllers(\_:animated:)

Replaces the view controllers currently managed by the navigation controller with the specified items.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setViewControllers(
    _ viewControllers: [UIViewController],
    animated: Bool
)
```

## Parameters 

`viewControllers`  

The view controllers to place in the stack. The front-to-back order of the controllers in this array represents the new bottom-to-top order of the controllers in the navigation stack. Thus, the last item added to the array becomes the top item of the navigation stack.

`animated`  

If true, animate the pushing or popping of the top view controller. If false, replace the view controllers without any animations.

## Discussion

Use this method to update or replace the current view controller stack without pushing or popping each controller explicitly. In addition, this method lets you update the set of controllers without animating the changes, which might be appropriate at launch time when you want to return the navigation controller to a previous state.

If animations are enabled, this method decides which type of transition to perform based on whether the last item in the `items` array is already in the navigation stack. If the view controller is currently in the stack, but is not the topmost item, this method uses a pop transition; if it is the topmost item, no transition is performed. If the view controller is not on the stack, this method uses a push transition. Only one transition is performed, but when that transition finishes, the entire contents of the stack are replaced with the new view controllers. For example, if controllers A, B, and C are on the stack and you set controllers D, A, and B, this method uses a pop transition and the resulting stack contains the controllers D, A, and B.

## See Also

### Accessing items on the navigation stack

var topViewController: UIViewController?

The view controller at the top of the navigation stack.

var visibleViewController: UIViewController?

The view controller associated with the currently visible view in the navigation interface.

var viewControllers: [UIViewController]

The view controllers currently on the navigation stack.

