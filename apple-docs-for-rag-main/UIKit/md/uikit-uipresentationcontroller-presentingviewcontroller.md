

- UIKit
- UIPresentationController
-  presentingViewController 

Instance Property

# presentingViewController

The view controller that is the starting point for the presentation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var presentingViewController: UIViewController { get }
```

## Discussion

The object in this property could be the root view controller of the window, a parent view controller that is marked as defining the current context, or the last view controller that was presented onscreen. This view controller may or may not be the same one whose present(_:animated:completion:) method was called to initiate the presentation process. It may also not be the view controller used to initialize your presentation controller.

## See Also

### Getting the presentation objects

var presentedViewController: UIViewController

The view controller being presented.

var containerView: UIView?

The view in which the presentation occurs.

var presentedView: UIView?

The view to be animated by the animator objects during a transition.

