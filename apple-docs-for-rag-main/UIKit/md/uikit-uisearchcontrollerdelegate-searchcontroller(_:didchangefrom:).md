

- UIKit
- UISearchControllerDelegate
-  searchController(\_:didChangeFrom:) 

Instance Method

# searchController(\_:didChangeFrom:)

Notifies the delegate after the search bar placement changes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
optional func searchController(
    _ searchController: UISearchController,
    didChangeFrom previousPlacement: UINavigationItem.SearchBarPlacement
)
```

## Parameters 

`searchController`  

The search controller associated with the search bar.

`previousPlacement`  

The previous search bar placement.

## Discussion

The system calls this method after a search bar placement change occurs. Implement this method if you need to make any custom changes to your search suggestions UI according to the previous search bar placement.

The system calls this method after searchController(_:willChangeTo:).

## See Also

### Responding to search bar placement updates

func searchController(UISearchController, willChangeTo: UINavigationItem.SearchBarPlacement)

Notifies the delegate before the search bar placement changes.

