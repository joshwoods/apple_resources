

- UIKit
-  UINavigationItem 

Class

# UINavigationItem

The items that a navigation bar displays when the associated view controller is visible.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UINavigationItem
```

## Overview

When building a navigation interface, each view controller that you push onto the navigation stack must have a UINavigationItem object that contains the buttons and views you want to display in the navigation bar. The managing UINavigationController object uses the navigation items of the topmost two view controllers to populate the navigation bar with content.

A navigation item always reflects information about its associated view controller. The navigation item must provide a title to display when the view controller is topmost on the navigation stack. The item can also contain additional buttons to display on the right (or trailing) side of the navigation bar. You can specify buttons and views to display on the left (or leading) side of the toolbar using the leftBarButtonItems property, but the navigation controller displays those buttons only when space is available.

The backBarButtonItem property of a navigation item reflects the Back button you want to display when the current view controller is just below the topmost view controller. The Back button doesn’t appear when the current view controller is topmost.

When specifying buttons for a navigation item, you must use UIBarButtonItem objects. If you want to display custom views in the navigation bar, you must wrap those views inside a UIBarButtonItem object before adding them to the navigation item.

## Topics

### Initializing an item

init(title: String)

Creates a navigation item with the specified title.

init?(coder: NSCoder)

Creates a navigation item from data in an unarchiver.

### Configuring the title

var title: String?

The navigation item’s title that displays in the navigation bar.

var largeTitleDisplayMode: UINavigationItem.LargeTitleDisplayMode

The mode for displaying the title of the navigation bar.

enum LargeTitleDisplayMode

Constants that indicate how to size the title of this item.

### Configuring the Back button

var backBarButtonItem: UIBarButtonItem?

The bar button item for adding a Back button to the navigation bar.

var backButtonTitle: String?

The custom title of the Back button.

var backButtonDisplayMode: UINavigationItem.BackButtonDisplayMode

The display mode of the Back button.

enum BackButtonDisplayMode

Constants that describe the display modes of the Back button.

var hidesBackButton: Bool

A Boolean value that determines whether the navigation item hides the Back button.

func setHidesBackButton(Bool, animated: Bool)

Hides or shows the Back button, optionally animating the transition.

var backAction: UIAction?

The back action for the navigation bar.

### Specifying the navigation style

var style: UINavigationItem.ItemStyle

A style that determines how the content of the navigation item lays out in the navigation bar.

enum ItemStyle

Constants that determine how the content of the navigation item lays out in the navigation bar.

### Specifying custom views

var centerItemGroups: [UIBarButtonItemGroup]

Customizable item groups to display in the center section of the navigation bar.

var leadingItemGroups: [UIBarButtonItemGroup]

Item groups to display in the leading section of the navigation bar.

var trailingItemGroups: [UIBarButtonItemGroup]

Item groups to display in the trailing section of the navigation bar.

var pinnedTrailingGroup: UIBarButtonItemGroup?

The item group to display on the trailing edge of the navigation bar, on the trailing side of the overflow and search items.

var titleView: UIView?

A custom view that displays in the center of the navigation bar when the receiver is the top item.

var leftBarButtonItems: [UIBarButtonItem]?

An array of custom bar button items to display on the left (or leading) side of the navigation bar when the navigation item is the top item.

var leftBarButtonItem: UIBarButtonItem?

A custom bar button item that displays on the left (or leading) edge of the navigation bar when the navigation item is the top item.

var rightBarButtonItems: [UIBarButtonItem]?

An array of custom bar button items to display on the right (or trailing) side of the navigation bar when the navigation item is the top item.

var rightBarButtonItem: UIBarButtonItem?

A custom bar button item that displays on the right (or trailing) edge of the navigation bar when the navigation item is the top item.

func setLeftBarButtonItems([UIBarButtonItem]?, animated: Bool)

Sets the left bar button items, optionally animating the transition to the new items.

func setLeftBarButton(UIBarButtonItem?, animated: Bool)

Sets the custom bar button item, optionally animating the transition to the new item.

func setRightBarButtonItems([UIBarButtonItem]?, animated: Bool)

Sets the right bar button items, optionally animating the transition to the new items.

func setRightBarButton(UIBarButtonItem?, animated: Bool)

Sets the custom bar button item, optionally animating the transition to the view.

### Getting and setting properties

var prompt: String?

A single line of text that displays at the top of the navigation bar.

var leftItemsSupplementBackButton: Bool

A Boolean value that indicates whether the left items display in addition to the Back button.

### Overriding the navigation bar’s appearance settings

var standardAppearance: UINavigationBarAppearance?

The appearance settings for a standard-height navigation bar.

var compactAppearance: UINavigationBarAppearance?

The appearance settings for a compact-height navigation bar.

var scrollEdgeAppearance: UINavigationBarAppearance?

The appearance settings for a standard-height navigation bar when the edge of scrollable content aligns with the edge of the navigation bar.

var compactScrollEdgeAppearance: UINavigationBarAppearance?

The appearance settings for a compact-height navigation bar when the edge of scrollable content aligns with the edge of the navigation bar.

### Integrating search into your interface

var searchController: UISearchController?

The search controller to integrate into your navigation interface.

var hidesSearchBarWhenScrolling: Bool

A Boolean value that indicates whether the app hides the integrated search bar when scrolling any underlying content.

var searchBarPlacement: UINavigationItem.SearchBarPlacement

The placement of the search bar in the navigation bar.

var preferredSearchBarPlacement: UINavigationItem.SearchBarPlacement

The preferred placement of the search bar in the navigation bar.

enum SearchBarPlacement

Constants that determine where the search bar appears in the navigation bar.

### Supporting navigation bar customization

var customizationIdentifier: String?

A globally unique string that enables user customization of the navigation bar layout.

### Working with the overflow menu

var additionalOverflowItems: UIDeferredMenuElement?

Additional items to present in the overflow menu.

var overflowPresentationSource: (any UIPopoverPresentationControllerSourceItem)?

The item you can use as an anchor to present a custom UI from the overflow menu button.

### Customizing the title menu

var titleMenuProvider: (([UIMenuElement]) -> UIMenu?)?

A closure that generates the navigation item’s title menu.

var documentProperties: UIDocumentProperties?

An object that provides the document header for the title menu.

class UIDocumentProperties

Information that UIKit uses to generate a document header for a navigation item’s title menu.

### Renaming documents

var renameDelegate: (any UINavigationItemRenameDelegate)?

The delegate for renaming the navigation item.

protocol UINavigationItemRenameDelegate

Methods an object implements to rename a navigation item.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- Sendable

## See Also

### Container view controllers

Creating a custom container view controller

Create a composite interface by combining content from one or more view controllers with other custom views.

class UISplitViewController

A container view controller that implements a hierarchical interface.

class UINavigationController

A container view controller that defines a stack-based scheme for navigating hierarchical content.

class UINavigationBar

Navigational controls that display in a bar along the top of the screen, usually in conjunction with a navigation controller.

class UITabBarController

A container view controller that manages a multiselection interface, where the selection determines which child view controller to display.

class UITabBar

A control that displays one or more buttons in a tab bar for selecting between different subtasks, views, or modes in an app.

class UITabBarItem

An object that describes an item in a tab bar.

class UITab

An object that manages a tab in a tab bar.

class UISearchTab

A tab subclass that represents the system’s search tab.

class UITabGroup

An object that manages a collection of tab objects.

class UIPageViewController

A container view controller that manages navigation between pages of content, where a subview controller manages each page.

