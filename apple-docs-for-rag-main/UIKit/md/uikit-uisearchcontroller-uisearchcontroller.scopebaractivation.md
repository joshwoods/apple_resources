

- UIKit
- UISearchController
-  UISearchController.ScopeBarActivation 

Enumeration

# UISearchController.ScopeBarActivation

Constants that specify the modes for showing and hiding the scope bar.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
enum ScopeBarActivation
```

## Overview

You use these constants with the scopeBarActivation property.

## Topics

### Constants

case automatic

A mode in which the system automatically determines when to show and hide the scope bar.

case manual

A mode that gives you manual control over when to show and hide the scope bar.

case onTextEntry

A mode in which the search controller shows the scope bar when typing begins in the search field, and hides it after search cancellation.

case onSearchActivation

A mode in which the search controller shows the scope bar when search becomes active, and hides it after search cancellation.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the search interface

var obscuresBackgroundDuringPresentation: Bool

A Boolean indicating whether to obscure the underlying content during a search.

var hidesNavigationBarDuringPresentation: Bool

A Boolean indicating whether to hide the navigation bar when searching.

var automaticallyShowsCancelButton: Bool

A Boolean indicating whether the search controller manages the visibility of the search bar’s cancel button.

var automaticallyShowsSearchResultsController: Bool

A Boolean indicating whether the search controller manages the visibility of its results controller.

var showsSearchResultsController: Bool

A Boolean indicating whether the search results controller is visible when the search controller is active.

var searchBarPlacement: UINavigationItem.SearchBarPlacement

The placement of the search bar in the navigation bar.

var ignoresSearchSuggestionsForSearchBarPlacementStacked: Bool

A Boolean value you use to specify whether the search controller prevents search suggestions from displaying for a stacked search bar.

var automaticallyShowsScopeBar: Bool

A Boolean indicating whether the search controller manages the visibility of the search bar’s scope bar.

Deprecated

var scopeBarActivation: UISearchController.ScopeBarActivation

A mode that determines when the search controller shows and hides the scope bar.

