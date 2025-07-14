

- UIKit
- UIPresentationController
-  containerView 

Instance Property

# containerView

The view in which the presentation occurs.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var containerView: UIView? { get }
```

## Discussion

UIKit sets the value of this property shortly after receiving the presentation controller from your transitioning delegate. The container view is always an ancestor of the presented view controller’s view. During transition animations, the container view also contains the presenting view controller’s view. When adding custom views to a presentation, add them to the container view.

If your transition also employs custom animator objects, those objects can get this container view from the containerView property of the context object provided by UIKit.

## See Also

### Getting the presentation objects

var presentingViewController: UIViewController

The view controller that is the starting point for the presentation.

var presentedViewController: UIViewController

The view controller being presented.

var presentedView: UIView?

The view to be animated by the animator objects during a transition.

