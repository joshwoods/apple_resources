

- UIKit
- UIPresentationController
-  presentedViewController 

Instance Property

# presentedViewController

The view controller being presented.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var presentedViewController: UIViewController { get }
```

## Discussion

This object corresponds to the one passed as the first parameter of the present(_:animated:completion:) method. The successful conclusion of the presentation process causes this view controller’s content to be displayed onscreen.

## See Also

### Getting the presentation objects

var presentingViewController: UIViewController

The view controller that is the starting point for the presentation.

var containerView: UIView?

The view in which the presentation occurs.

var presentedView: UIView?

The view to be animated by the animator objects during a transition.

