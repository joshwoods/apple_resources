

- UIKit
- UICellAccessory
-  UICellAccessory.DisclosureIndicatorOptions 

Structure

# UICellAccessory.DisclosureIndicatorOptions

Configuration options for a disclosure indicator.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
struct DisclosureIndicatorOptions
```

## Topics

### Creating configuration options

init(isHidden: Bool?, reservedLayoutWidth: UICellAccessory.LayoutDimension?, tintColor: UIColor?)

Creates a disclosure indicator options structure.

### Accessing configuration options

var isHidden: Bool

A Boolean value that determines whether the cell hides the accessory.

var reservedLayoutWidth: UICellAccessory.LayoutDimension

The layout width that the system reserves for the accessory, and then centers the accessory within.

var tintColor: UIColor?

The tint color to apply to the accessory.

## See Also

### Creating a disclosure indicator

static func disclosureIndicator(displayed: UICellAccessory.DisplayedState, options: UICellAccessory.DisclosureIndicatorOptions) -> UICellAccessory

Creates a disclosure indicator system accessory with the specified display state and configuration options.

