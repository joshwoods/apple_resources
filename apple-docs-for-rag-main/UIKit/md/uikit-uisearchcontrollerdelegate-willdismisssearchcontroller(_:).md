

- UIKit
- UISearchControllerDelegate
-  willDismissSearchController(\_:) 

Instance Method

# willDismissSearchController(\_:)

Notifies the delegate that the system is about to automatically dismiss the search controller.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func willDismissSearchController(_ searchController: UISearchController)
```

## Parameters 

`searchController`  

The UISearchController object to dismiss.

## Discussion

The system only calls this method when it’s about to automatically dismiss the search controller. The system doesn’t call this method if you explicitly dismiss the search controller.

## See Also

### Presenting and dismissing the search controller

func didDismissSearchController(UISearchController)

Notifies the delegate when the system completes automatic dismissal of the search controller.

func didPresentSearchController(UISearchController)

Notifies the delegate when the system completes automatic presentation of the search controller.

func presentSearchController(UISearchController)

Presents the designated search controller.

func willPresentSearchController(UISearchController)

Notifies the delegate that the system is about to automatically display the search controller.

