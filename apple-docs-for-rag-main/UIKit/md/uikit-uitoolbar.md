

- UIKit
-  UIToolbar 

Class

# UIToolbar

A control that displays one or more buttons along the bottom edge of your interface.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIToolbar
```

## Overview

To create toolbar items, use the UIBarButtonItem class. To add toolbar items to a toolbar, use the setItems(_:animated:) method.

Toolbar images that represent normal and highlighted states of an item derive from the image you set using the inherited image property from the UIBarItem class. The toolbar’s tintColor colors the image.

If you need radio button style controls, use the UITabBar class instead of UIToolbar.

### Customize appearance

You use the methods listed in Customizing appearance to customize the appearance of toolbars. You send the setter messages to the appearance proxy (`[UIToolbar appearance]`) to customize all toolbars, or to a specific `UIToolbar` instance. When a property is dependent on the bar metrics, you should typically specify a value for UIBarMetrics.default as well as for landscapePhone.

## Topics

### Managing toolbar changes

var delegate: (any UIToolbarDelegate)?

The toolbar’s delegate object.

protocol UIToolbarDelegate

The interface that toolbar delegate objects implement to manage the toolbar behavior.

### Configuring toolbar items

var items: [UIBarButtonItem]?

The items displayed on the toolbar.

func setItems([UIBarButtonItem]?, animated: Bool)

Sets the items on the toolbar by animating the changes.

### Customizing appearance

var standardAppearance: UIToolbarAppearance

The appearance settings to use for a standard-height toolbar.

var compactAppearance: UIToolbarAppearance?

The appearance settings to use for a compact-height toolbar.

var scrollEdgeAppearance: UIToolbarAppearance?

The appearance settings for a standard-height toolbar when the edge of scrollable content aligns with the edge of the toolbar.

var compactScrollEdgeAppearance: UIToolbarAppearance?

The appearance settings for a compact-height toolbar when the edge of any scrollable content aligns with the edge of a compact-height toolbar.

var isTranslucent: Bool

A Boolean value that indicates whether the toolbar is translucent.

Legacy customizations

Customize appearance information directly on the toolbar object.

## Relationships

### Inherits From

- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UIBarPositioning
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Bars

class UIBarItem

An abstract superclass for items that you can add to a bar that appears at the bottom of the screen.

class UIBarButtonItem

A specialized button for placement on a toolbar, navigation bar, or shortcuts bar.

class UIBarButtonItemGroup

A group of one or more bar button items for placement on a navigation bar or shortcuts bar.

class UINavigationBar

Navigational controls that display in a bar along the top of the screen, usually in conjunction with a navigation controller.

class UISearchBar

A specialized view for receiving search-related information from the user.

class UITabBar

A control that displays one or more buttons in a tab bar for selecting between different subtasks, views, or modes in an app.

class UITabBarItem

An object that describes an item in a tab bar.

protocol UIBarPositioning

A set of methods for defining the positioning of bars in iOS apps.

protocol UIBarPositioningDelegate

A set of methods that support the positioning of a bar that conforms to the UIBarPositioning protocol.

