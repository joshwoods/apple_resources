

- UIKit
- UICellAccessory
-  UICellAccessory.CheckmarkOptions 

Structure

# UICellAccessory.CheckmarkOptions

Configuration options for a checkmark accessory.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
struct CheckmarkOptions
```

## Topics

### Creating configuration options

init(isHidden: Bool?, reservedLayoutWidth: UICellAccessory.LayoutDimension?, tintColor: UIColor?)

Creates a checkmark accessory options structure.

### Accessing configuration options

var isHidden: Bool

A Boolean value that determines whether the cell hides the accessory.

var reservedLayoutWidth: UICellAccessory.LayoutDimension

The layout width that the system reserves for the accessory, and then centers the accessory within.

var tintColor: UIColor?

The tint color to apply to the accessory.

## See Also

### Creating a checkmark accessory

static func checkmark(displayed: UICellAccessory.DisplayedState, options: UICellAccessory.CheckmarkOptions) -> UICellAccessory

Creates a checkmark system accessory with the specified display state and configuration options.

