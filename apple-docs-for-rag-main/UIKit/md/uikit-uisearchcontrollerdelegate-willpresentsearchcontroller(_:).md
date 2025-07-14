

- UIKit
- UISearchControllerDelegate
-  willPresentSearchController(\_:) 

Instance Method

# willPresentSearchController(\_:)

Notifies the delegate that the system is about to automatically display the search controller.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func willPresentSearchController(_ searchController: UISearchController)
```

## Parameters 

`searchController`  

The UISearchController object to present.

## Discussion

The system only calls this method when it’s about to automatically present the search controller. The system doesn’t call this method when you explicitly present the search controller.

## See Also

### Presenting and dismissing the search controller

func didDismissSearchController(UISearchController)

Notifies the delegate when the system completes automatic dismissal of the search controller.

func didPresentSearchController(UISearchController)

Notifies the delegate when the system completes automatic presentation of the search controller.

func presentSearchController(UISearchController)

Presents the designated search controller.

func willDismissSearchController(UISearchController)

Notifies the delegate that the system is about to automatically dismiss the search controller.

