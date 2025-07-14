

- UIKit
- UIViewControllerContextTransitioning
-  containerView 

Instance Property

# containerView

The view that acts as the superview for the views involved in the transition.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var containerView: UIView { get }
```

**Required**

## Return Value

The view that contains both views involved in the transition.

## Discussion

The container view acts as the superview of all other views (including those of the presenting and presented view controllers) during the animation sequence. UIKit sets this view for you and automatically adds the view of the presenting view controller to it. The animator object is responsible for adding the view of the presented view controller, and the animator object or presentation controller must use this view as the container for all other views involved in the transition.

## See Also

### Accessing the transition objects

func viewController(forKey: UITransitionContextViewControllerKey) -> UIViewController?

Returns a view controller involved in the transition.

**Required**

func view(forKey: UITransitionContextViewKey) -> UIView?

Returns the specified view involved in the transition.

**Required**

