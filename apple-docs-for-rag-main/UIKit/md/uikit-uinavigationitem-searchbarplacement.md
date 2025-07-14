

- UIKit
- UINavigationItem
-  searchBarPlacement 

Instance Property

# searchBarPlacement

The placement of the search bar in the navigation bar.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var searchBarPlacement: UINavigationItem.SearchBarPlacement { get }
```

## Discussion

Use this property to determine the actual search bar placement when the preferredSearchBarPlacement is UINavigationItem.SearchBarPlacement.automatic.

This property only applies when the navigation item has a searchController.

## See Also

### Integrating search into your interface

var searchController: UISearchController?

The search controller to integrate into your navigation interface.

var hidesSearchBarWhenScrolling: Bool

A Boolean value that indicates whether the app hides the integrated search bar when scrolling any underlying content.

var preferredSearchBarPlacement: UINavigationItem.SearchBarPlacement

The preferred placement of the search bar in the navigation bar.

enum SearchBarPlacement

Constants that determine where the search bar appears in the navigation bar.

