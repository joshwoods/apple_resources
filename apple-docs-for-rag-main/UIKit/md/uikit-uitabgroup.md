

- UIKit
-  UITabGroup 

Class

# UITabGroup

An object that manages a collection of tab objects.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
class UITabGroup
```

## Mentioned in 

Elevating your iPad app with a tab bar and sidebar

## Overview

Use tab groups to create a rich hierarchy of tab items. On iPad, the system displays the tab group as a section in the sidebar. For more information, see Elevating your iPad app with a tab bar and sidebar.

## Topics

### Creating tab groups

init(title: String, image: UIImage?, identifier: String, children: [UITab], viewControllerProvider: ((UITab) -> UIViewController)?)

Creates a tab group.

### Accessing tabs

var children: [UITab]

The tabs within a tab group.

func tab(forIdentifier: String) -> UITab?

Returns a tab with a matching identifier, if any.

var defaultChildIdentifier: String?

The identifier for the default subitem.

var selectedChild: UITab?

The currently selected tab.

### Configuring a tab group

var sidebarAppearance: UITabGroup.SidebarAppearance

The appearance of a tab group’s section in a sidebar.

enum SidebarAppearance

The appearance of a section in a sidebar.

var managingNavigationController: UINavigationController?

The controller that manages navigation for items in a sidebar.

### Managing customization

var allowsReordering: Bool

A Boolean value that indicates people can reorder subitems in the sidebar.

var displayOrderIdentifiers: [String]

An array that contains the identifiers of subitems in their display order.

var displayOrder: [UITab]

An array that contains instances of subitems in their display order.

### Assigning actions

var sidebarActions: [UIAction]

An array of actions that appear in a section in a sidebar.

## Relationships

### Inherits From

- UITab

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable
- UIAccessibilityIdentification
- UIPopoverPresentationControllerSourceItem
- UISpringLoadedInteractionSupporting

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

class UINavigationItem

The items that a navigation bar displays when the associated view controller is visible.

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

class UIPageViewController

A container view controller that manages navigation between pages of content, where a subview controller manages each page.

