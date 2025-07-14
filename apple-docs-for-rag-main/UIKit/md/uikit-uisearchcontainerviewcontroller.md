

- UIKit
-  UISearchContainerViewController 

Class

# UISearchContainerViewController

A view controller that manages the presentation of search results in your interface.

iOS 9.1+iPadOS 9.1+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
class UISearchContainerViewController
```

## Overview

In tvOS, rather than push a UISearchController onto a navigation controller’s stack or use one as a child of another container view controller, embed an instance of this class and let it manage the presentation of the search controller’s content.

UISearchContainerViewController presents its UISearchController, instead of containing it. So implement view appearance methods, such as viewWillAppear(_:) and didMove(toParent:) on both view controllers.

## Topics

### Creating a search container view controller

init(searchController: UISearchController)

Initializes and returns a search container view controller with the specified search controller object.

### Getting the search controller

var searchController: UISearchController

The search controller the search container view controller manages.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Search interface

class UISearchController

A view controller that manages the display of search results based on interactions with a search bar.

class UISearchBar

A specialized view for receiving search-related information from the user.

protocol UISearchResultsUpdating

A set of methods that let you update search results based on information the user enters into the search bar.

Displaying searchable content by using a search controller

Create a user interface with searchable content in a table view.

Using suggested searches with a search controller

Create a search interface with a table view of suggested searches.

