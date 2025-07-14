

- UIKit
- UICellAccessory
-  UICellAccessory.InsertOptions 

Structure

# UICellAccessory.InsertOptions

Configuration options for an insert accessory.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
struct InsertOptions
```

## Topics

### Creating configuration options

init(isHidden: Bool?, reservedLayoutWidth: UICellAccessory.LayoutDimension?, tintColor: UIColor?, backgroundColor: UIColor?)

Creates an insert accessory options structure.

### Accessing configuration options

var isHidden: Bool

A Boolean value that determines whether the cell hides the accessory.

var reservedLayoutWidth: UICellAccessory.LayoutDimension

The layout width that the system reserves for the accessory, and then centers the accessory within.

var tintColor: UIColor?

The tint color to apply to the accessory.

var backgroundColor: UIColor?

The background color to apply to the accessory.

## See Also

### Creating an insert accessory

static func insert(displayed: UICellAccessory.DisplayedState, options: UICellAccessory.InsertOptions, actionHandler: UICellAccessory.ActionHandler?) -> UICellAccessory

Creates an insert system accessory with the specified display state, configuration options, and optional action handler.

