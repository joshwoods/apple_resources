

- UIKit
-  UICellAccessory 

Structure

# UICellAccessory

An accessory in a collection view list cell.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
struct UICellAccessory
```

## Overview

A cell accessory is a visual element that you can add to a list cell (UICollectionViewListCell). You use a cell accessory as a visual indicator or to let a user perform a cell-specific action like selecting, reordering, or deleting the cell. A cell accessory appears either on the leading or the trailing edge of a cell, outside of the cell’s content view.

UIKit defines a set of standard system cell accessories. System accessories have default system-defined appearances, but you can make some customizations to them, like setting a custom tint color. You can’t customize the placement of system accessories. If you want additional customization, you can create a custom accessory with customView(configuration:).

You add accessories to a list cell by setting its accessories array.

```
cell.accessories = [ 
    .checkmark(), 
    .disclosureIndicator(options: .init(tintColor: .systemGray)), 
    .delete(),
    .reorder() 
]
```

Important

The system throws an exception if you include more than one instance of any system accessory. You can include multiple custom accessories.

## Topics

### Creating a disclosure indicator

static func disclosureIndicator(displayed: UICellAccessory.DisplayedState, options: UICellAccessory.DisclosureIndicatorOptions) -> UICellAccessory

Creates a disclosure indicator system accessory with the specified display state and configuration options.

struct DisclosureIndicatorOptions

Configuration options for a disclosure indicator.

### Creating an outline disclosure

static func outlineDisclosure(displayed: UICellAccessory.DisplayedState, options: UICellAccessory.OutlineDisclosureOptions, actionHandler: UICellAccessory.ActionHandler?) -> UICellAccessory

Creates an outline disclosure system accessory with the specified display state, configuration options, and optional action handler.

struct OutlineDisclosureOptions

Configuration options for an outline disclosure.

### Creating a popup menu accessory

static func popUpMenu(UIMenu, displayed: UICellAccessory.DisplayedState, options: UICellAccessory.PopUpMenuOptions, selectedElementDidChangeHandler: UICellAccessory.MenuSelectedElementDidChangeHandler?) -> UICellAccessory

Creates a popup menu system accessory with the specified menu, display state, configuration options, and optional selection handler.

typealias MenuSelectedElementDidChangeHandler

A closure type that defines a handler to perform when a user selects an element in the menu.

struct PopUpMenuOptions

Configuration options for a popup menu accessory.

### Creating a checkmark accessory

static func checkmark(displayed: UICellAccessory.DisplayedState, options: UICellAccessory.CheckmarkOptions) -> UICellAccessory

Creates a checkmark system accessory with the specified display state and configuration options.

struct CheckmarkOptions

Configuration options for a checkmark accessory.

### Creating a delete accessory

static func delete(displayed: UICellAccessory.DisplayedState, options: UICellAccessory.DeleteOptions, actionHandler: UICellAccessory.ActionHandler?) -> UICellAccessory

Creates a delete system accessory with the specified display state, configuration options, and optional action handler.

struct DeleteOptions

Configuration options for a delete accessory.

### Creating an insert accessory

static func insert(displayed: UICellAccessory.DisplayedState, options: UICellAccessory.InsertOptions, actionHandler: UICellAccessory.ActionHandler?) -> UICellAccessory

Creates an insert system accessory with the specified display state, configuration options, and optional action handler.

struct InsertOptions

Configuration options for an insert accessory.

### Creating a reorder accessory

static func reorder(displayed: UICellAccessory.DisplayedState, options: UICellAccessory.ReorderOptions) -> UICellAccessory

Creates a reorder system accessory with the specified display state and configuration options.

struct ReorderOptions

Configuration options for a reorder accessory.

### Creating a multiselect accessory

static func multiselect(displayed: UICellAccessory.DisplayedState, options: UICellAccessory.MultiselectOptions) -> UICellAccessory

Creates a multiselect system accessory with the specified display state and configuration options.

struct MultiselectOptions

Configuration options for a multiselect accessory.

### Creating a label accessory

static func label(text: String, displayed: UICellAccessory.DisplayedState, options: UICellAccessory.LabelOptions) -> UICellAccessory

Creates a label system accessory with the specified text, display state, and configuration options.

struct LabelOptions

Configuration options for a label accessory.

### Creating a detail accessory

static func detail(displayed: UICellAccessory.DisplayedState, options: UICellAccessory.DetailOptions, actionHandler: UICellAccessory.ActionHandler?) -> UICellAccessory

Creates a detail system accessory with the specified display state, configuration options, and optional action handler.

struct DetailOptions

Configuration options for a detail accessory.

### Creating a custom accessory

static func customView(configuration: UICellAccessory.CustomViewConfiguration) -> UICellAccessory

Creates a custom view accessory.

struct CustomViewConfiguration

Configuration options for a custom accessory.

### Checking the accessory’s type

let accessoryType: UICellAccessory.AccessoryType

The type of the cell accessory.

enum AccessoryType

Constants that describe the type of the cell accessory.

### Customizing appearance and placement

enum LayoutDimension

Constants that describe the layout dimension for the accessory.

enum Placement

Constants that describe the placement of the accessory within the cell.

enum DisplayedState

Constants that describe the cell-editing states that the accessory appears in.

### Performing accessory actions

typealias ActionHandler

A closure that the system calls when a user taps a cell accessory.

## See Also

### Managing cell accessories

var accessories: [UICellAccessory]

An array of the accessories that decorate the cell.

