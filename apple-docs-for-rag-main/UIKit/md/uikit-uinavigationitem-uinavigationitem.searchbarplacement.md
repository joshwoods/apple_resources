

- UIKit
- UINavigationItem
-  UINavigationItem.SearchBarPlacement 

Enumeration

# UINavigationItem.SearchBarPlacement

Constants that determine where the search bar appears in the navigation bar.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
enum SearchBarPlacement
```

## Overview

Use these constants to specify the placement of the search bar that belongs to the navigation item’s search controller (searchController).

## Topics

### Constants

case automatic

A constant that places the search bar according to the current layout.

case inline

A constant that places the search bar on the trailing edge of the navigation bar, inline with the other content.

case stacked

A constant that stacks the search bar vertically below the other content in the navigation bar.

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

### Integrating search into your interface

var searchController: UISearchController?

The search controller to integrate into your navigation interface.

var hidesSearchBarWhenScrolling: Bool

A Boolean value that indicates whether the app hides the integrated search bar when scrolling any underlying content.

var searchBarPlacement: UINavigationItem.SearchBarPlacement

The placement of the search bar in the navigation bar.

var preferredSearchBarPlacement: UINavigationItem.SearchBarPlacement

The preferred placement of the search bar in the navigation bar.

