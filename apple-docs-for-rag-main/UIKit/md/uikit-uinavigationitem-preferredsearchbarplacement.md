

- UIKit
- UINavigationItem
-  preferredSearchBarPlacement 

Instance Property

# preferredSearchBarPlacement

The preferred placement of the search bar in the navigation bar.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var preferredSearchBarPlacement: UINavigationItem.SearchBarPlacement { get set }
```

## Mentioned in 

Building a desktop-class iPad app

## Discussion

Use this property to specify the search bar placement. If the value of the property is UINavigationItem.SearchBarPlacement.automatic, use the searchBarPlacement property to determine the actual placement. The default value of this property is UINavigationItem.SearchBarPlacement.automatic.

This property only applies when the navigation item has a searchController.

## See Also

### Integrating search into your interface

var searchController: UISearchController?

The search controller to integrate into your navigation interface.

var hidesSearchBarWhenScrolling: Bool

A Boolean value that indicates whether the app hides the integrated search bar when scrolling any underlying content.

var searchBarPlacement: UINavigationItem.SearchBarPlacement

The placement of the search bar in the navigation bar.

enum SearchBarPlacement

Constants that determine where the search bar appears in the navigation bar.

