

- UIKit
- UICellAccessory
-  UICellAccessory.ReorderOptions 

Structure

# UICellAccessory.ReorderOptions

Configuration options for a reorder accessory.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
struct ReorderOptions
```

## Topics

### Creating configuration options

init(isHidden: Bool?, reservedLayoutWidth: UICellAccessory.LayoutDimension?, tintColor: UIColor?, showsVerticalSeparator: Bool?)

Creates a reorder accessory options structure.

### Accessing configuration options

var isHidden: Bool

A Boolean value that determines whether the cell hides the accessory.

var reservedLayoutWidth: UICellAccessory.LayoutDimension

The layout width that the system reserves for the accessory, and then centers the accessory within.

var tintColor: UIColor?

The tint color to apply to the accessory.

var showsVerticalSeparator: Bool

A Boolean value that determines whether a vertical separator displays before the accessory when it appears after another accessory.

## See Also

### Creating a reorder accessory

static func reorder(displayed: UICellAccessory.DisplayedState, options: UICellAccessory.ReorderOptions) -> UICellAccessory

Creates a reorder system accessory with the specified display state and configuration options.

