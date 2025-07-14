

- UIKit
-  UISearchControllerDelegate 

Protocol

# UISearchControllerDelegate

A set of delegate methods for search controller objects.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UISearchControllerDelegate : NSObjectProtocol
```

## Topics

### Presenting and dismissing the search controller

func didDismissSearchController(UISearchController)

Notifies the delegate when the system completes automatic dismissal of the search controller.

func didPresentSearchController(UISearchController)

Notifies the delegate when the system completes automatic presentation of the search controller.

func presentSearchController(UISearchController)

Presents the designated search controller.

func willDismissSearchController(UISearchController)

Notifies the delegate that the system is about to automatically dismiss the search controller.

func willPresentSearchController(UISearchController)

Notifies the delegate that the system is about to automatically display the search controller.

### Responding to search bar placement updates

func searchController(UISearchController, didChangeFrom: UINavigationItem.SearchBarPlacement)

Notifies the delegate after the search bar placement changes.

func searchController(UISearchController, willChangeTo: UINavigationItem.SearchBarPlacement)

Notifies the delegate before the search bar placement changes.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to presentation and dismissal

var delegate: (any UISearchControllerDelegate)?

The search controller’s delegate.

