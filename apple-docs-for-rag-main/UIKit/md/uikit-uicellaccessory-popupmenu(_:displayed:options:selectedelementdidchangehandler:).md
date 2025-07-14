

- UIKit
- UICellAccessory
-  popUpMenu(\_:displayed:options:selectedElementDidChangeHandler:) 

Type Method

# popUpMenu(\_:displayed:options:selectedElementDidChangeHandler:)

Creates a popup menu system accessory with the specified menu, display state, configuration options, and optional selection handler.

iOS 16.0+iPadOS 16.0+Mac CatalysttvOS 14.0+visionOS

``` source
static func popUpMenu(
    _ menu: UIMenu,
    displayed: UICellAccessory.DisplayedState = .always,
    options: UICellAccessory.PopUpMenuOptions = PopUpMenuOptions(),
    selectedElementDidChangeHandler: UICellAccessory.MenuSelectedElementDidChangeHandler? = nil
) -> UICellAccessory
```

## Parameters 

`menu`  

The menu to display when a user taps the popup menu accessory.

`displayed`  

The cell-editing states that the popup menu accessory appears in. This parameter has a default value of UICellAccessory.DisplayedState.always.

`options`  

Configuration options for the popup menu accessory. See UICellAccessory.PopUpMenuOptions for possible configuration options.

`selectedElementDidChangeHandler`  

An optional closure that the system calls when a user selects an element in the menu.

## Return Value

A configured popup menu cell accessory that appears as a pair of chevrons that point upward and downward. This accessory indicates that tapping anywhere in the cell presents a popup menu. This accessory appears on the trailing edge of the cell.

## See Also

### Creating a popup menu accessory

typealias MenuSelectedElementDidChangeHandler

A closure type that defines a handler to perform when a user selects an element in the menu.

struct PopUpMenuOptions

Configuration options for a popup menu accessory.

