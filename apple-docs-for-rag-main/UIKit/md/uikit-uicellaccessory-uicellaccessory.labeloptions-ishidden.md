

- UIKit
- UICellAccessory
- UICellAccessory.LabelOptions
-  isHidden 

Instance Property

# isHidden

A Boolean value that determines whether the cell hides the accessory.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var isHidden: Bool
```

## Discussion

A hidden accessory takes up space in the layout, but it isn’t visible and doesn’t provide any behaviors.

Use this property to achieve a consistent layout across cells when some cells show this type of accessory and others don’t.

## See Also

### Accessing configuration options

var reservedLayoutWidth: UICellAccessory.LayoutDimension

The layout width that the system reserves for the accessory, and then centers the accessory within.

var tintColor: UIColor?

The tint color to apply to the accessory.

var font: UIFont

The font for the label.

var adjustsFontForContentSizeCategory: Bool

A Boolean value that determines whether the label automatically adjusts its font according to the content size category.

