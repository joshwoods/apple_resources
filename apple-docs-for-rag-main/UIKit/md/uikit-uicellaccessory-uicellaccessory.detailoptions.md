

- UIKit
- UICellAccessory
-  UICellAccessory.DetailOptions 

Structure

# UICellAccessory.DetailOptions

Configuration options for a detail accessory.

iOS 15.4+iPadOS 15.4+Mac CatalysttvOS 15.4+visionOS

``` source
struct DetailOptions
```

## Topics

### Creating configuration options

init(isHidden: Bool?, reservedLayoutWidth: UICellAccessory.LayoutDimension?, tintColor: UIColor?)

Creates a detail accessory options structure.

### Accessing configuration options

var isHidden: Bool

A Boolean value that determines whether the cell hides the accessory.

var reservedLayoutWidth: UICellAccessory.LayoutDimension

The layout width that the system reserves for the accessory, and then centers the accessory within.

var tintColor: UIColor?

The tint color to apply to the accessory.

## See Also

### Creating a detail accessory

static func detail(displayed: UICellAccessory.DisplayedState, options: UICellAccessory.DetailOptions, actionHandler: UICellAccessory.ActionHandler?) -> UICellAccessory

Creates a detail system accessory with the specified display state, configuration options, and optional action handler.

