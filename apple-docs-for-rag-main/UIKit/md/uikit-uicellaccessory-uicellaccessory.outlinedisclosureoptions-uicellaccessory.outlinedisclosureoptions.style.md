

- UIKit
- UICellAccessory
- UICellAccessory.OutlineDisclosureOptions
-  UICellAccessory.OutlineDisclosureOptions.Style 

Enumeration

# UICellAccessory.OutlineDisclosureOptions.Style

Constants that describe the style of the outline disclosure accessory.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
enum Style
```

## Topics

### Constants

case automatic

The system automatically determines the style depending on whether the cell’s configuration is as a section header.

case cell

The style to use for a selectable cell with nested children.

case header

The style to use for a section header.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Accessing configuration options

var isHidden: Bool

A Boolean value that determines whether the cell hides the accessory.

var reservedLayoutWidth: UICellAccessory.LayoutDimension

The layout width that the system reserves for the accessory, and then centers the accessory within.

var tintColor: UIColor?

The tint color to apply to the accessory.

var style: UICellAccessory.OutlineDisclosureOptions.Style

The style of the outline disclosure accessory.

