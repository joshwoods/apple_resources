

- UIKit
-  UITabBarItem 

Class

# UITabBarItem

An object that describes an item in a tab bar.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UITabBarItem
```

## Overview

A tab bar item is a segment of a tab bar that represents a specific section of your app. A tab bar displays one or more items that allow the user to switch between the different sections. The user can select one item at a time.

The most common approach for displaying a tab bar is to use a tab bar controller. The controller’s tab bar displays an item for each view controller you provide when you set the viewControllers property or call the setViewControllers(_:animated:) method. You’re responsible for supplying the tab bar items. Do this by setting each view controller’s tabBarItem property. When the user selects an item, the tab bar controller displays its view controller. For more information, see UITabBarController.

You can also use a tab bar independent of a tab bar controller. After creating a tab bar, add it to your view hierarchy. Provide the items by setting the tab bar’s items property or by using the setItems(_:animated:) method. In this configuration, you’re responsible for updating the view hierarchy to display the correct content. Use UITabBarDelegate to know when the selection changes. For more information, see UITabBar.

The system provides several tab bar items for common use cases. If you need a custom item, create one with a title and an image. You can further customize the item by providing an alternate image that appears when the user selects it. By default, the item doesn’t display the images you provide. Instead, it generates new images from the alpha values of your images and tints them. To prevent this, provide images that use the UIImage.RenderingMode.alwaysOriginal rendering mode.

An item can adjust its appearance when in certain conditions. For example, you can specify different appearances for inline and compact inline layouts or for when the item’s state changes. To do this, set the item’s standardAppearance property. If you don’t want this behavior, you can set the individual properties on the item instead.

A tab bar item can display a supplementary value in a badge that provides extra information to the user. For example, the Phone app uses a badge’s value to display the number of missed calls. You can customize the badge’s appearance, including its background color and text attributes.

## Topics

### Creating a tab bar item

convenience init(tabBarSystemItem: UITabBarItem.SystemItem, tag: Int)

Creates a tab bar item using a system-provided configuration.

convenience init(title: String?, image: UIImage?, tag: Int)

Creates a tab bar item that displays a title and an image.

convenience init(title: String?, image: UIImage?, selectedImage: UIImage?)

Creates a tab bar item that toggles the image it displays when its selected state changes.

init()

Creates a tab bar item with a default configuration.

init?(coder: NSCoder)

Creates a tab bar item from a serialized instance.

enum SystemItem

Constants that represent the system tab bar items.

### Configuring the item’s appearance

var selectedImage: UIImage?

The source image the item uses to generate its selected image.

var standardAppearance: UITabBarAppearance?

The appearance settings for a tab bar.

var scrollEdgeAppearance: UITabBarAppearance?

The appearance settings for the tab bar when the edge of scrollable content aligns with the edge of the tab bar.

var titlePositionAdjustment: UIOffset

The offset to apply to the title’s position.

### Configuring the item’s badge

var badgeValue: String?

The text that the item’s badge displays.

var badgeColor: UIColor?

The background color of the item’s badge.

func setBadgeTextAttributes([NSAttributedString.Key : Any]?, for: UIControl.State)

Registers text attributes that the badge uses for the specified state.

func badgeTextAttributes(for: UIControl.State) -> [NSAttributedString.Key : Any]?

Returns the badge’s text attributes for the specified state.

## Relationships

### Inherits From

- UIBarItem

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- Sendable
- UIAccessibilityIdentification
- UIAppearance
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

class UITab

An object that manages a tab in a tab bar.

class UISearchTab

A tab subclass that represents the system’s search tab.

class UITabGroup

An object that manages a collection of tab objects.

class UIPageViewController

A container view controller that manages navigation between pages of content, where a subview controller manages each page.

