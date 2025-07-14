

- UIKit
- UINavigationItem
-  hidesSearchBarWhenScrolling 

Instance Property

# hidesSearchBarWhenScrolling

A Boolean value that indicates whether the app hides the integrated search bar when scrolling any underlying content.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var hidesSearchBarWhenScrolling: Bool { get set }
```

## Discussion

When the value of this property is true, the search bar is visible only when the scroll position equals the top of your content view. When the user scrolls down, the search bar collapses into the navigation bar. Scrolling back to the top reveals the search bar again. When the value of this property is false, the search bar remains regardless of the current scroll position.

You must configure the searchController property for this property to have any effect. The navigation controller hides and shows only the search bar provided by the search controller in that property.

## See Also

### Integrating search into your interface

var searchController: UISearchController?

The search controller to integrate into your navigation interface.

var searchBarPlacement: UINavigationItem.SearchBarPlacement

The placement of the search bar in the navigation bar.

var preferredSearchBarPlacement: UINavigationItem.SearchBarPlacement

The preferred placement of the search bar in the navigation bar.

enum SearchBarPlacement

Constants that determine where the search bar appears in the navigation bar.

