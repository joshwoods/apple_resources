

- UIKit
- UISearchController
-  delegate 

Instance Property

# delegate

The search controller’s delegate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var delegate: (any UISearchControllerDelegate)? { get set }
```

## Discussion

Use the delegate object to receive notifications when the search results controller is presented and dismissed. You might use these notifications to customize the search interface or perform related actions.

## See Also

### Responding to presentation and dismissal

protocol UISearchControllerDelegate

A set of delegate methods for search controller objects.

