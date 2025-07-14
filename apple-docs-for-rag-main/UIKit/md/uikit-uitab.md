

- UIKit
-  UITab 

Class

# UITab

An object that manages a tab in a tab bar.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
class UITab
```

## Mentioned in 

Elevating your iPad app with a tab bar and sidebar

## Overview

To create a tab, call init(title:image:identifier:viewControllerProvider:). In the closure, return the view controller your app presents when someone selects the tab. Then pass an array of tabs to your UITabBarController object’s tabs property.

For more information, see Elevating your iPad app with a tab bar and sidebar.

## Topics

### Creating tabs

init(title: String, image: UIImage?, identifier: String, viewControllerProvider: ((UITab) -> UIViewController)?)

Creates a tab object.

### Accessing a tab’s appearance

var title: String

A tab’s title.

var subtitle: String?

A tab’s subtitle.

var identifier: String

A string identifier for a tab.

var image: UIImage?

A tab’s image.

var badgeValue: String?

A tab’s badge value.

var viewController: UIViewController?

The view controller that the system presents when someone selects a tab.

### Managing customization

var isHidden: Bool

A Boolean value that indicates whether an item is hidden in a sidebar.

var isHiddenByDefault: Bool

A Boolean value that indicates whether an item is hidden by default.

var allowsHiding: Bool

A Boolean value that indicates whether people can hide a tab in a sidebar.

var preferredPlacement: UITab.Placement

The preferred placement for a tab when displayed in contexts that allow different placement.

enum Placement

A tab’s placement when displayed in contexts that allow different placement.

### Accessing context

var parent: UITabGroup?

The containing tab group.

var tabBarController: UITabBarController?

The containing tab bar controller.

var userInfo: Any?

A custom object associated with the tab.

### Instance Properties

var hasVisiblePlacement: Bool

Determines if the tab has a visible placement. Returns YES if the tab is visible in a tab bar that supports different tab placements. Otherwise returns NO.

var isEnabled: Bool

Determines if the tab is enabled. When NO, tabs will have a disabled appearance and cannot be selected by the user. Default is YES.

var managingTabGroup: UITabGroup?

The managing tab group for the tab. This returns the rootmost `UITabGroup` in the tab’s parent hierarchy with an active `managingNavigationController`. This can be different to `parent` if the tab is nested in multiple levels of tab groups. If the tab does not belong to a hierarchy with a managing navigation controller, then this will return nil. Default is nil.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UISearchTab
- UITabGroup

### Conforms To

- CVarArg
- Copyable
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

class UISearchTab

A tab subclass that represents the system’s search tab.

class UITabGroup

An object that manages a collection of tab objects.

class UIPageViewController

A container view controller that manages navigation between pages of content, where a subview controller manages each page.

