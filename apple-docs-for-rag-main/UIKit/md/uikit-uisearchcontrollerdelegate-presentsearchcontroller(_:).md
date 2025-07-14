

- UIKit
- UISearchControllerDelegate
-  presentSearchController(\_:) 

Instance Method

# presentSearchController(\_:)

Presents the designated search controller.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func presentSearchController(_ searchController: UISearchController)
```

## Parameters 

`searchController`  

The UISearchController object to present.

## Discussion

The system calls this method when the user begins editing in the search controller, or you set the isActive property to true. The system performs a default presentation if you don’t implement this method or you present the controller yourself.

## See Also

### Presenting and dismissing the search controller

func didDismissSearchController(UISearchController)

Notifies the delegate when the system completes automatic dismissal of the search controller.

func didPresentSearchController(UISearchController)

Notifies the delegate when the system completes automatic presentation of the search controller.

func willDismissSearchController(UISearchController)

Notifies the delegate that the system is about to automatically dismiss the search controller.

func willPresentSearchController(UISearchController)

Notifies the delegate that the system is about to automatically display the search controller.

