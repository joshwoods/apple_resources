

- UIKit
- UICellAccessory
-  UICellAccessory.OutlineDisclosureOptions 

Structure

# UICellAccessory.OutlineDisclosureOptions

Configuration options for an outline disclosure.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
struct OutlineDisclosureOptions
```

## Topics

### Creating configuration options

init(style: UICellAccessory.OutlineDisclosureOptions.Style?, isHidden: Bool?, reservedLayoutWidth: UICellAccessory.LayoutDimension?, tintColor: UIColor?)

Creates an outline disclosure options structure.

### Accessing configuration options

var isHidden: Bool

A Boolean value that determines whether the cell hides the accessory.

var reservedLayoutWidth: UICellAccessory.LayoutDimension

The layout width that the system reserves for the accessory, and then centers the accessory within.

var tintColor: UIColor?

The tint color to apply to the accessory.

var style: UICellAccessory.OutlineDisclosureOptions.Style

The style of the outline disclosure accessory.

enum Style

Constants that describe the style of the outline disclosure accessory.

## See Also

### Creating an outline disclosure

static func outlineDisclosure(displayed: UICellAccessory.DisplayedState, options: UICellAccessory.OutlineDisclosureOptions, actionHandler: UICellAccessory.ActionHandler?) -> UICellAccessory

Creates an outline disclosure system accessory with the specified display state, configuration options, and optional action handler.

