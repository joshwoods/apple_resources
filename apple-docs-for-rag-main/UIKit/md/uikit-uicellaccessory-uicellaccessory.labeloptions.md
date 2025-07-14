

- UIKit
- UICellAccessory
-  UICellAccessory.LabelOptions 

Structure

# UICellAccessory.LabelOptions

Configuration options for a label accessory.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
struct LabelOptions
```

## Topics

### Creating configuration options

init(isHidden: Bool?, reservedLayoutWidth: UICellAccessory.LayoutDimension?, tintColor: UIColor?, font: UIFont?, adjustsFontForContentSizeCategory: Bool?)

Creates a label accessory options structure.

### Accessing configuration options

var isHidden: Bool

A Boolean value that determines whether the cell hides the accessory.

var reservedLayoutWidth: UICellAccessory.LayoutDimension

The layout width that the system reserves for the accessory, and then centers the accessory within.

var tintColor: UIColor?

The tint color to apply to the accessory.

var font: UIFont

The font for the label.

var adjustsFontForContentSizeCategory: Bool

A Boolean value that determines whether the label automatically adjusts its font according to the content size category.

## See Also

### Creating a label accessory

static func label(text: String, displayed: UICellAccessory.DisplayedState, options: UICellAccessory.LabelOptions) -> UICellAccessory

Creates a label system accessory with the specified text, display state, and configuration options.

