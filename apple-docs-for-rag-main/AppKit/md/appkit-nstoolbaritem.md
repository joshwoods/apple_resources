

- AppKit
-  NSToolbarItem 

Class

# NSToolbarItem

A single item that appears in a window’s toolbar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
class NSToolbarItem
```

## Overview

An NSToolbarItem object displays an image and text string in the toolbar area of a window. You can also create toolbar items that display custom views you provide. Toolbar items provide fast access to common commands or features in the window. For example, the Finder window uses toolbar items to help someone navigate the file system.

You typically create toolbar items at the same time you create your window’s toolbar. The system provides some standard items like spacers you can include in your toolbar. It also provides items that display standard interfaces like the color panel or font panel. For any custom toolbar items you create, provide an action method to call when someone clicks the item.

You can display your toolbar item’s content using a custom view if you prefer, rather than an image and text label. If you specify an NSSearchField object for the view, the system automatically adjusts the minimum and maximum size of the search field to the system-standard values.

## Topics

### Creating a toolbar item

init(itemIdentifier: NSToolbarItem.Identifier)

Creates a toolbar item with the specified identifier.

convenience init(itemIdentifier: NSToolbarItem.Identifier, barButtonItem: UIBarButtonItem)

Creates a toolbar item with property values from the specified bar button item.

### Getting the toolbar item’s identity

var itemIdentifier: NSToolbarItem.Identifier

The value you use to identify the toolbar item.

struct Identifier

Constants for the standard toolbar items that the system provides.

### Describing the item

var possibleLabels: Set&lt;String>

The set of labels that the item might display.

var label: String

The label that appears for this item in the toolbar.

var paletteLabel: String

The label that appears when the toolbar item is in the customization palette.

var title: String

The title of the toolbar item.

var toolTip: String?

The tooltip to display when someone hovers over the item in the toolbar.

### Getting the item’s visual appearance

var image: UIImage?

The image to display for the toolbar item.

var view: NSView?

The custom view you use to draw the toolbar item.

### Performing the item’s action

var target: AnyObject?

The object that defines the action method the toolbar item calls when clicked.

var action: Selector?

The action method to call when someone clicks on the toolbar item.

### Configuring the item’s menu

var menuFormRepresentation: NSMenuItem?

The menu item to use when the toolbar item is in the overflow menu.

var itemMenuFormRepresentation: UIMenuElement?

The menu item to use for the toolbar item is in the overflow menu in a Mac app built with Mac Catalyst.

### Getting the item’s configuration

var isVisible: Bool

A Boolean value that indicates whether the item is currently visible in the toolbar, and not in the overflow menu.

var isBordered: Bool

A Boolean value that indicates whether the toolbar item has a bordered style.

var isNavigational: Bool

A Boolean value that indicates whether the item behaves as a navigation item in the toolbar.

var isEnabled: Bool

A Boolean value that indicates whether the item is enabled.

var allowsDuplicatesInToolbar: Bool

A Boolean value that indicates whether the toolbar item can appear more than once in a toolbar.

Deprecated

var visibilityPriority: NSToolbarItem.VisibilityPriority

The display priority associated with the toolbar item.

struct VisibilityPriority

Constants that indicate which toolbar items to keep in the toolbar when space is limited.

var tag: Int

An integer tag you can use to identify the toolbar item.

### Getting the parent toolbar

var toolbar: NSToolbar?

The toolbar that currently includes the item.

### Validating the item

var autovalidates: Bool

A Boolean value that indicates whether the toolbar automatically validates the item.

func validate()

Validates the toolbar item’s menu and its ability to perfrom its action.

### Deprecated

var minSize: NSSize

The toolbar item’s minimum size.

Deprecated

var maxSize: NSSize

The toolbar item’s maximum size.

Deprecated

### Instance Properties

var isHidden: Bool

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSMenuToolbarItem
- NSSearchToolbarItem
- NSSharingServicePickerToolbarItem
- NSToolbarItemGroup
- NSTrackingSeparatorToolbarItem

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMenuItemValidation
- NSObjectProtocol
- NSValidatedUserInterfaceItem
- Sendable
- UIPopoverPresentationControllerSourceItem

## See Also

### Items

class NSToolbarItemGroup

A group of subitems in a toolbar item.

enum ControlRepresentation

enum SelectionMode

A value that indicates how a grouped toolbar item selects its subitems.

class NSMenuToolbarItem

A control that presents a menu in a window’s toolbar.

class NSSearchToolbarItem

A toolbar item that contains a search field optimized for performing text-based searches.

class NSTrackingSeparatorToolbarItem

A toolbar separator that aligns with the vertical split view in the same window.

