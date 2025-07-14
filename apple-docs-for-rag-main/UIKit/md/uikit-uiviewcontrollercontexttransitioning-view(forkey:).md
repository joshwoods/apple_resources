

- UIKit
- UIViewControllerContextTransitioning
-  view(forKey:) 

Instance Method

# view(forKey:)

Returns the specified view involved in the transition.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func view(forKey key: UITransitionContextViewKey) -> UIView?
```

**Required**

## Parameters 

`key`  

The key identifying the view you want. For a list of possible keys, see `View Transition Keys`.

## Return Value

The view object for the specified key or `nil` if the view could not be found.

## Discussion

The view returned by this method may or may not be the root view of the corresponding view controller. A situation where the views may not be the same is when a system-provided presentation controller installs another view underneath the presented view controller’s view.

## See Also

### Accessing the transition objects

var containerView: UIView

The view that acts as the superview for the views involved in the transition.

**Required**

func viewController(forKey: UITransitionContextViewControllerKey) -> UIViewController?

Returns a view controller involved in the transition.

**Required**

