

- UIKit
- UICellAccessory
- UICellAccessory.LabelOptions
-  reservedLayoutWidth 

Instance Property

# reservedLayoutWidth

The layout width that the system reserves for the accessory, and then centers the accessory within.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var reservedLayoutWidth: UICellAccessory.LayoutDimension
```

## Discussion

Use this property to ensure consistent horizontal alignment from both system and custom accessories to your content, even when the accessories vary in size.

The reserved layout width only affects the amount of space for the accessory, and its positioning within that space. It doesn’t affect the size of the accessory.

## See Also

### Accessing configuration options

var isHidden: Bool

A Boolean value that determines whether the cell hides the accessory.

var tintColor: UIColor?

The tint color to apply to the accessory.

var font: UIFont

The font for the label.

var adjustsFontForContentSizeCategory: Bool

A Boolean value that determines whether the label automatically adjusts its font according to the content size category.

