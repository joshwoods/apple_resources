

- UIKit
- UICellAccessory
-  UICellAccessory.PopUpMenuOptions 

Structure

# UICellAccessory.PopUpMenuOptions

Configuration options for a popup menu accessory.

iOS 16.0+iPadOS 16.0+Mac CatalysttvOS 14.0+visionOS

``` source
struct PopUpMenuOptions
```

## Topics

### Creating configuration options

init(isHidden: Bool?, reservedLayoutWidth: UICellAccessory.LayoutDimension?, tintColor: UIColor?)

Creates a popup menu accessory options structure.

### Accessing configuration options

var isHidden: Bool

A Boolean value that determines whether the cell hides the accessory.

var reservedLayoutWidth: UICellAccessory.LayoutDimension

The layout width that the system reserves for the accessory, and then centers the accessory within.

var tintColor: UIColor?

The tint color to apply to the accessory.

## See Also

### Creating a popup menu accessory

static func popUpMenu(UIMenu, displayed: UICellAccessory.DisplayedState, options: UICellAccessory.PopUpMenuOptions, selectedElementDidChangeHandler: UICellAccessory.MenuSelectedElementDidChangeHandler?) -> UICellAccessory

Creates a popup menu system accessory with the specified menu, display state, configuration options, and optional selection handler.

typealias MenuSelectedElementDidChangeHandler

A closure type that defines a handler to perform when a user selects an element in the menu.

