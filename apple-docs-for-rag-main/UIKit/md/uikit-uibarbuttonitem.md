

- UIKit
-  UIBarButtonItem 

Class

# UIBarButtonItem

A specialized button for placement on a toolbar, navigation bar, or shortcuts bar.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIBarButtonItem
```

## Overview

You typically use Interface Builder to create and configure bar button items. However, you can customize the appearance of buttons by sending the setter messages to UIBarButtonItemAppearance to customize all buttons, or to a specific UIBarButtonItem instance. You can use customized buttons in standard places in a UINavigationItem object or a UIToolbar instance.

In general, specify a value for the normal state so that other states without a custom value set can use it. Similarly, when a property depends on the bar metrics (for instance, on the iPhone in landscape orientation, bars have a different height from the standard), specify a value of UIBarMetrics.default.

## Topics

### Creating items

convenience init(title: String?, image: UIImage?, primaryAction: UIAction?, menu: UIMenu?)

Creates a plain-style item using the specified title, image, primary action, and context menu.

convenience init(title: String?, image: UIImage?, target: AnyObject?, action: Selector?, menu: UIMenu?)

Creates a plain-style item using the specified title, image, target, action, and context menu.

init()

Initializes the item to its default state.

init?(coder: NSCoder)

Creates an item from data in an unarchiver.

### Creating items of a specific style

convenience init(title: String?, style: UIBarButtonItem.Style, target: Any?, action: Selector?)

Creates an item using the specified title, style, target, and action.

convenience init(image: UIImage?, style: UIBarButtonItem.Style, target: Any?, action: Selector?)

Creates an item using the specified image, style, target, and action.

convenience init(image: UIImage?, landscapeImagePhone: UIImage?, style: UIBarButtonItem.Style, target: Any?, action: Selector?)

Creates an item using the specified images, style, target, and action.

### Creating system items

convenience init(systemItem: UIBarButtonItem.SystemItem, primaryAction: UIAction?, menu: UIMenu?)

Creates an item using the specified system item, primary action, and context menu.

convenience init(barButtonSystemItem: UIBarButtonItem.SystemItem, target: Any?, action: Selector?)

Creates an item using the specified system item, target, and action.

enum SystemItem

Constants that define system-supplied images for bar button items.

### Creating custom items

convenience init(customView: UIView)

Creates an item using the specified custom view.

### Creating space items

class func fixedSpace(CGFloat) -> Self

Creates a new fixed-width space item.

class func flexibleSpace() -> Self

Creates a new flexible-width space item.

### Creating groups

func creatingOptionalGroup(customizationIdentifier: String, isInDefaultCustomization: Bool) -> UIBarButtonItemGroup

Places the item in an optional group that a person can move, add to, or remove from the navigation bar during layout customization.

func creatingFixedGroup() -> UIBarButtonItemGroup

Places the item in a fixed group that a person can’t move or remove from the navigation bar during layout customization.

func creatingMovableGroup(customizationIdentifier: String) -> UIBarButtonItemGroup

Places the item in a movable group that a person can move but can’t remove from the navigation bar during layout customization.

### Managing the custom view

var customView: UIView?

A custom view representing the item.

### Managing the action

var primaryAction: UIAction?

The action associated with the item.

var changesSelectionAsPrimaryAction: Bool

A Boolean value that indicates whether the button represents an action or selection.

var action: Selector?

The selector defining the action message to send to the target object when the user taps this bar button item.

var target: AnyObject?

The object that receives an action when the user selects the item.

### Managing the context menu

var menu: UIMenu?

The context menu for this button.

var preferredMenuElementOrder: UIContextMenuConfiguration.ElementOrder

The preferred menu-element ordering strategy for the menu.

### Customizing item appearance

var style: UIBarButtonItem.Style

The style of the item.

enum Style

Constants that specify the style of an item.

var tintColor: UIColor?

The tint color to apply to the button item.

var isHidden: Bool

A Boolean that determines the visibility of the item.

var isSelected: Bool

A Boolean value that indicates whether the button is in a selected state.

var width: CGFloat

The width of the item.

var possibleTitles: Set&lt;String>?

The set of possible titles to display on the bar button.

### Customizing the Back button

func backButtonBackgroundImage(for: UIControl.State, barMetrics: UIBarMetrics) -> UIImage?

Returns the back button background image for a specified control state and bar metrics.

func setBackButtonBackgroundImage(UIImage?, for: UIControl.State, barMetrics: UIBarMetrics)

Sets the back button background image for a specified control state and bar metrics.

func backButtonTitlePositionAdjustment(for: UIBarMetrics) -> UIOffset

Returns the back button title offset for specified bar metrics.

func setBackButtonTitlePositionAdjustment(UIOffset, for: UIBarMetrics)

Sets the back button title offset for specified bar metrics.

func backButtonBackgroundVerticalPositionAdjustment(for: UIBarMetrics) -> CGFloat

Returns the back button vertical position offset for specified bar metrics.

func setBackButtonBackgroundVerticalPositionAdjustment(CGFloat, for: UIBarMetrics)

Sets the back button vertical position offset for specified bar metrics.

### Customizing the background

func backgroundVerticalPositionAdjustment(for: UIBarMetrics) -> CGFloat

Returns the background vertical position offset for specified bar metrics.

func setBackgroundVerticalPositionAdjustment(CGFloat, for: UIBarMetrics)

Sets the background vertical position offset for specified bar metrics.

func backgroundImage(for: UIControl.State, barMetrics: UIBarMetrics) -> UIImage?

Returns the background image for a specified state and bar metrics.

func setBackgroundImage(UIImage?, for: UIControl.State, barMetrics: UIBarMetrics)

Sets the background image for a specified state and bar metrics.

func backgroundImage(for: UIControl.State, style: UIBarButtonItem.Style, barMetrics: UIBarMetrics) -> UIImage?

Returns the background image for the specified state, style, and metrics.

func setBackgroundImage(UIImage?, for: UIControl.State, style: UIBarButtonItem.Style, barMetrics: UIBarMetrics)

Sets the background image for the specified state, style, and metrics.

### Customizing the title placement

func titlePositionAdjustment(for: UIBarMetrics) -> UIOffset

Returns the title offset for specified bar metrics.

func setTitlePositionAdjustment(UIOffset, for: UIBarMetrics)

Sets the title offset for specified bar metrics.

### Configuring symbol effects

var isSymbolAnimationEnabled: Bool

A Boolean value that indicates whether symbol effects animate.

func addSymbolEffect(some IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Adds an indefinite symbol effect to the bar button item with the specified options and animation.

func addSymbolEffect(some DiscreteSymbolEffect &amp; IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Adds a discrete, indefinite symbol effect to the bar button item with the specified options and animation.

func addSymbolEffect(some DiscreteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Adds a discrete symbol effect to the bar button item with the specified options and animation.

func setSymbolImage(UIImage, contentTransition: some ContentTransitionSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions)

Sets a symbol image using the specified content-transition effect and options.

func removeSymbolEffect(ofType: some IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Removes the symbol effect that matches the specified indefinite effect type, using the specified options and animation setting.

func removeSymbolEffect(ofType: some DiscreteSymbolEffect &amp; IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Removes the symbol effect that matches the specified discrete, indefinite effect type, using the specified options and animation setting.

func removeSymbolEffect(ofType: some DiscreteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Removes the symbol effect that matches the specified discrete effect type, using the specified options and animation setting.

func removeAllSymbolEffects(options: SymbolEffectOptions, animated: Bool)

Removes all symbol effects from the bar button item, using the specified options and animation setting.

### Getting the group

var buttonGroup: UIBarButtonItemGroup?

The group that the button belongs to.

### Representing the item in a menu

var menuRepresentation: UIMenuElement?

A menu element that represents the item when it appears in a menu.

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
- UIAccessibilityIdentification
- UIAppearance
- UIPopoverPresentationControllerSourceItem
- UISpringLoadedInteractionSupporting

## See Also

### Bars

class UIBarItem

An abstract superclass for items that you can add to a bar that appears at the bottom of the screen.

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

