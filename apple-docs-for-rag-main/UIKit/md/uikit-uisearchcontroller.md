

- UIKit
-  UISearchController 

Class

# UISearchController

A view controller that manages the display of search results based on interactions with a search bar.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UISearchController
```

## Overview

Use a search controller to provide a standard search experience of the contents of another view controller. When the user interacts with a UISearchBar, the search controller coordinates with a search results controller to display the search results.

In iOS, incorporate the search controller’s searchBar into your own view controller’s interface. Display your view controller in whatever way is appropriate for your app. See Displaying searchable content by using a search controller and Using suggested searches with a search controller to learn how to implement a search controller in your app.

In tvOS, start with a UISearchContainerViewController to manage the presentation of the search controller. See UIKit Catalog (tvOS): Creating and Customizing UIKit Controls to learn how to implement a search controller embedded inside a `UISearchContainerViewController` object.

Note

Don’t use a UISearchContainerViewController in iOS.

### Display search results

Specify a second view controller for displaying search results when you call init(searchResultsController:). When the user interacts with the search bar, the search controller automatically displays the results controller with the results you specify. If your results view is full-screen in tvOS, set the searchControllerObservedScrollView to the results controller as well, so the search bar scrolls with your content view.

Provide a UISearchResultsUpdating object to the search controller’s searchResultsUpdater property. Typically, the view controller with your searchable content also acts as the search results updater object, but you can use another object if you prefer. When the user interacts with the search bar, the search controller calls the appropriate UISearchResultsUpdating method, giving your object the opportunity to perform the search and update the contents of your search results view.

### Customize transitions

To customize the presentation or dismissal of the search results controller, set the search controller’s delegate property to an object that conforms to the UISearchControllerDelegate protocol. Then implement delegate methods in this object to receive presentation and dismissal events from the search controller.

## Topics

### Creating a search controller

init(searchResultsController: UIViewController?)

Creates and returns a search controller with the specified view controller for displaying the results.

init?(coder: NSCoder)

Returns an initialized search controller from data in the specified unarchiver.

init(nibName: String?, bundle: Bundle?)

Returns an initialized view controller with the nib file in the specified bundle.

### Responding to presentation and dismissal

var delegate: (any UISearchControllerDelegate)?

The search controller’s delegate.

protocol UISearchControllerDelegate

A set of delegate methods for search controller objects.

### Managing the search results

var searchBar: UISearchBar

The search bar to install in your interface.

var searchResultsUpdater: (any UISearchResultsUpdating)?

The object responsible for updating the contents of the search results controller.

var searchResultsController: UIViewController?

The view controller that displays the results of the search.

var isActive: Bool

The presented state of the search interface.

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

enum ScopeBarActivation

Constants that specify the modes for showing and hiding the scope bar.

### Providing search suggestions

var searchSuggestions: [any UISearchSuggestion]?

A list of suggestions to offer as shortcuts below the search field.

var ignoresSearchSuggestionsForSearchBarPlacementStacked: Bool

A Boolean value you use to specify whether the search controller prevents search suggestions from displaying for a stacked search bar.

class UISearchSuggestionItem

A selectable search parameter.

protocol UISearchSuggestion

A set of attributes that a selectable search suggestion must provide.

### Deprecated

var searchControllerObservedScrollView: UIScrollView?

The view with which the controller coordinates scrolling animations.

Deprecated

var dimsBackgroundDuringPresentation: Bool

A Boolean indicating whether to dim the underlying content during a search.

Deprecated

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
- UIViewControllerAnimatedTransitioning
- UIViewControllerTransitioningDelegate

## See Also

### Search interface

class UISearchContainerViewController

A view controller that manages the presentation of search results in your interface.

class UISearchBar

A specialized view for receiving search-related information from the user.

protocol UISearchResultsUpdating

A set of methods that let you update search results based on information the user enters into the search bar.

Displaying searchable content by using a search controller

Create a user interface with searchable content in a table view.

Using suggested searches with a search controller

Create a search interface with a table view of suggested searches.

