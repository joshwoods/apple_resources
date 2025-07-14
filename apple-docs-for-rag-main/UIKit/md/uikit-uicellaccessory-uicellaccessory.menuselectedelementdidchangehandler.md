

- UIKit
- UICellAccessory
-  UICellAccessory.MenuSelectedElementDidChangeHandler 

Type Alias

# UICellAccessory.MenuSelectedElementDidChangeHandler

A closure type that defines a handler to perform when a user selects an element in the menu.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
typealias MenuSelectedElementDidChangeHandler = (UIMenu) -> Void
```

## See Also

### Creating a popup menu accessory

static func popUpMenu(UIMenu, displayed: UICellAccessory.DisplayedState, options: UICellAccessory.PopUpMenuOptions, selectedElementDidChangeHandler: UICellAccessory.MenuSelectedElementDidChangeHandler?) -> UICellAccessory

Creates a popup menu system accessory with the specified menu, display state, configuration options, and optional selection handler.

struct PopUpMenuOptions

Configuration options for a popup menu accessory.

