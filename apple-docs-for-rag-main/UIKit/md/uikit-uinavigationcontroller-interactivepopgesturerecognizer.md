

- UIKit
- UINavigationController
-  interactivePopGestureRecognizer 

Instance Property

# interactivePopGestureRecognizer

The gesture recognizer responsible for popping the top view controller off the navigation stack.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var interactivePopGestureRecognizer: UIGestureRecognizer? { get }
```

## Discussion

The navigation controller installs this gesture recognizer on its view and uses it to pop the topmost view controller off the navigation stack. You can use this property to retrieve the gesture recognizer and tie it to the behavior of other gesture recognizers in your user interface. When tying your gesture recognizers together, make sure they recognize their gestures simultaneously to ensure that your gesture recognizers are given a chance to handle the event.

## See Also

### Related Documentation

func gestureRecognizer(UIGestureRecognizer, shouldRecognizeSimultaneouslyWith: UIGestureRecognizer) -> Bool

Asks the delegate if two gesture recognizers should be allowed to recognize gestures simultaneously.

### Pushing and popping stack items

func pushViewController(UIViewController, animated: Bool)

Pushes a view controller onto the receiver’s stack and updates the display.

func popViewController(animated: Bool) -> UIViewController?

Pops the top view controller from the navigation stack and updates the display.

func popToRootViewController(animated: Bool) -> [UIViewController]?

Pops all the view controllers on the stack except the root view controller and updates the display.

func popToViewController(UIViewController, animated: Bool) -> [UIViewController]?

Pops view controllers until the specified view controller is at the top of the navigation stack.

