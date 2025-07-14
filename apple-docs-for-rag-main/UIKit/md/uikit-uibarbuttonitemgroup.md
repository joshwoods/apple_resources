

- UIKit
-  UIBarButtonItemGroup 

Class

# UIBarButtonItemGroup

A group of one or more bar button items for placement on a navigation bar or shortcuts bar.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
class UIBarButtonItemGroup
```

## Overview

A group contains one or more bar button items and an optional representative item that’s displayed instead of the individual items under space constraints. You can create any number of groups and configure each group with any number of items.

When creating a group with more than one bar button item, it’s recommended that you also provide a representative item to display. The representative item must be a completely separate bar button item; it must not be one of the items already in the group. UIKit displays the representative item when there isn’t enough room to display all of the group’s items in the bar. Taps in the representative item call that item’s action method. When you don’t specify an action method, UIKit automatically displays the items in the group using a standard interface. To present your own interface, provide a custom action method and use it to display the interface you want.

### Support the shortcuts bar

After configuring a group, assign it to the UITextInputAssistantItem object associated with one of your app’s responder objects. Your custom items are displayed only in conjunction with the system keyboard. When the keyboard is displayed, UIKit retrieves your custom groups from the text input assistant item and adds the corresponding items to the shortcuts bar. You may specify more than one group before and after the typing suggestions. UIKit tries to display as many items as possible on the shortcuts bar, falling back to the groups’ representative items as needed.

## Topics

### Creating a group

class func fixedGroup(representativeItem: UIBarButtonItem?, items: [UIBarButtonItem]) -> UIBarButtonItemGroup

Creates a fixed group that a person can’t move or remove from the navigation bar during layout customization.

class func movableGroup(customizationIdentifier: String, representativeItem: UIBarButtonItem?, items: [UIBarButtonItem]) -> UIBarButtonItemGroup

Creates a movable group that a person can move but can’t remove from the navigation bar during layout customization.

class func optionalGroup(customizationIdentifier: String, isInDefaultCustomization: Bool, representativeItem: UIBarButtonItem?, items: [UIBarButtonItem]) -> UIBarButtonItemGroup

Creates an optional group that a person can move, add to, or remove from the navigation bar during layout customization.

init(barButtonItems: [UIBarButtonItem], representativeItem: UIBarButtonItem?)

Creates a fixed group with the specified items.

init?(coder: NSCoder)

Creates a bar button item group from data in an unarchiver.

### Configuring the group

var barButtonItems: [UIBarButtonItem]

The bar button items to display on the bar.

var representativeItem: UIBarButtonItem?

The item to display for a group when space is constrained.

var alwaysAvailable: Bool

A Boolean value that determines whether the group is always available through the UI.

### Determining the group’s appearance

var isDisplayingRepresentativeItem: Bool

A Boolean value indicating whether the representative item is showing in place of the group’s items.

var isHidden: Bool

A Boolean that determines the visibility of the group.

### Representing the group in a menu

var menuRepresentation: UIMenuElement?

A menu element that represents the group when it appears in a menu.

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

### Bars

class UIBarItem

An abstract superclass for items that you can add to a bar that appears at the bottom of the screen.

class UIBarButtonItem

A specialized button for placement on a toolbar, navigation bar, or shortcuts bar.

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

