

- UIKit
- UINavigationItem
-  searchController 

Instance Property

# searchController

The search controller to integrate into your navigation interface.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var searchController: UISearchController? { get set }
```

## Discussion

When a view controller in your navigation interface supports search, assign the corresponding search controller to this property. The navigation controller integrates the search bar from your search controller into the navigation bar interface, presenting a single bar for both search and navigation. Use the hidesSearchBarWhenScrolling property to control the visibility of the search bar when scrolling.

## See Also

### Integrating search into your interface

var hidesSearchBarWhenScrolling: Bool

A Boolean value that indicates whether the app hides the integrated search bar when scrolling any underlying content.

var searchBarPlacement: UINavigationItem.SearchBarPlacement

The placement of the search bar in the navigation bar.

var preferredSearchBarPlacement: UINavigationItem.SearchBarPlacement

The preferred placement of the search bar in the navigation bar.

enum SearchBarPlacement

Constants that determine where the search bar appears in the navigation bar.

