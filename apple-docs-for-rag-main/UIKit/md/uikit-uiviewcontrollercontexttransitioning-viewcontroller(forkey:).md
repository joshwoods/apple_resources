

- UIKit
- UIViewControllerContextTransitioning
-  viewController(forKey:) 

Instance Method

# viewController(forKey:)

Returns a view controller involved in the transition.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func viewController(forKey key: UITransitionContextViewControllerKey) -> UIViewController?
```

**Required**

## Parameters 

`key`  

The key identifying the view controller you want. For a list of possible keys, see `View Controller Transition Keys`.

## Return Value

The view controller object for the specified key or `nil` if the view controller could not be found.

## See Also

### Accessing the transition objects

var containerView: UIView

The view that acts as the superview for the views involved in the transition.

**Required**

func view(forKey: UITransitionContextViewKey) -> UIView?

Returns the specified view involved in the transition.

**Required**

