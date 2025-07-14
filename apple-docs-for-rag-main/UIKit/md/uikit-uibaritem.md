

- UIKit
-  UIBarItem 

Class

# UIBarItem

An abstract superclass for items that you can add to a bar that appears at the bottom of the screen.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIBarItem
```

## Overview

Items on a bar behave in a way similar to buttons (instances of UIButton). They have a title, image, action, and target. You can also enable and disable an item on a bar.

### Customize appearance

You can customize the image to represent the item, and the position of the image, using image and imageInsets respectively.

You can also specify a custom image and position to use in landscape orientation when using the iPhone appearance idiom using landscapeImagePhone and landscapeImagePhoneInsets respectively. In addition, you can customize the title’s text attributes using setTitleTextAttributes(_:for:), either for a single item, or for all items by using the appearance proxy (for example, `[UIBarItem appearance]`).

## Topics

### Creating a bar item

init()

Initializes the bar item to its default state.

init?(coder: NSCoder)

Creates a bar item from data in an unarchiver.

### Getting and setting properties

var title: String?

The title displayed on the item.

var image: UIImage?

The image used to represent the item.

var landscapeImagePhone: UIImage?

The image to use to represent the item in landscape orientation when using the iPhone appearance idiom.

var largeContentSizeImage: UIImage?

The image to display for users who are blind or have low vision.

var imageInsets: UIEdgeInsets

The image inset or outset for each edge.

var landscapeImagePhoneInsets: UIEdgeInsets

The image inset or outset for each edge of the image in landscape orientation when using the iPhone appearance idiom.

var largeContentSizeImageInsets: UIEdgeInsets

The insets to apply to the bar item’s large image when displaying the image in an assistive UI.

var isEnabled: Bool

A Boolean value indicating whether the item is enabled.

var tag: Int

The bar item’s tag, an app-supplied integer that you can use to identify bar item objects in your app.

### Customizing appearance

func setTitleTextAttributes([NSAttributedString.Key : Any]?, for: UIControl.State)

Sets the title’s text attributes for a given control state.

func titleTextAttributes(for: UIControl.State) -> [NSAttributedString.Key : Any]?

Returns the title’s text attributes for a given control state.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIBarButtonItem
- UITabBarItem

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

## See Also

### Bars

class UIBarButtonItem

A specialized button for placement on a toolbar, navigation bar, or shortcuts bar.

class UIBarButtonItemGroup

A group of one or more bar button items for placement on a navigation bar or shortcuts bar.

class UINavigationBar

Navigational controls that display in a bar along the top of the screen, usually in conjunction with a navigation controller.

class UISearchBar

A specialized view for receiving search-related information from the user.

class UIToolbar

A control that displays one or more buttons along the bottom edge of your interface.

class UITabBar

A control that displays one or more buttons in a tab bar for selecting between different subtasks, views, or modes in an app.

class UITabBarItem

An object that describes an item in a tab bar.

protocol UIBarPositioning

A set of methods for defining the positioning of bars in iOS apps.

protocol UIBarPositioningDelegate

A set of methods that support the positioning of a bar that conforms to the UIBarPositioning protocol.

