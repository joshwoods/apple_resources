

- UIKit
- UISearchControllerDelegate
-  searchController(\_:willChangeTo:) 

Instance Method

# searchController(\_:willChangeTo:)

Notifies the delegate before the search bar placement changes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
optional func searchController(
    _ searchController: UISearchController,
    willChangeTo newPlacement: UINavigationItem.SearchBarPlacement
)
```

## Parameters 

`searchController`  

The search controller associated with the search bar.

`newPlacement`  

The new search bar placement.

## Discussion

The system calls this method before a search bar placement change occurs, such as in response to a layout change that alters the amount of available space in the navigation bar. Implement this method if you need to make any custom changes to your search suggestions UI according to the new search bar placement.

The system calls this method before searchController(_:didChangeFrom:).

## See Also

### Responding to search bar placement updates

func searchController(UISearchController, didChangeFrom: UINavigationItem.SearchBarPlacement)

Notifies the delegate after the search bar placement changes.

