

- UIKit
- UINavigationController
-  delegate 

Instance Property

# delegate

The delegate of the navigation controller object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var delegate: (any UINavigationControllerDelegate)? { get set }
```

## Discussion

You can use the navigation delegate to perform additional actions in response to changes in the navigation interface. For more information about implementing the delegate, see UINavigationControllerDelegate.

## See Also

### Customizing the navigation interface behavior

protocol UINavigationControllerDelegate

The interface for an object that serves as a navigation controller’s delegate.

