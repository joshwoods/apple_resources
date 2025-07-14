

- UIKit
- UIPresentationController
-  presentedView 

Instance Property

# presentedView

The view to be animated by the animator objects during a transition.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var presentedView: UIView? { get }
```

## Return Value

The view to present. This view must be either the presented view controller’s view or an ancestor of that view.

## Discussion

The default implementation of this method returns the presented view controller’s view. If you want to animate a different view, you may override this method and return that view. The view you specify must either be the presented view controller’s view or must be one of its ancestors.

The view returned by this method is given to the animator objects, which are responsible for animating it onscreen. The animator objects retrieve the view using the view(forKey:) method of the context object provided by UIKit.

UIKit calls this method multiple times during the course of a presentation, so your implementation should return the appropriate view as quickly as possible. Do not use this method to actually configure your view hierarchy. If you intend to return a custom view, configure your view hierarchy in the presentationTransitionWillBegin() method.

## See Also

### Getting the presentation objects

var presentingViewController: UIViewController

The view controller that is the starting point for the presentation.

var presentedViewController: UIViewController

The view controller being presented.

var containerView: UIView?

The view in which the presentation occurs.

