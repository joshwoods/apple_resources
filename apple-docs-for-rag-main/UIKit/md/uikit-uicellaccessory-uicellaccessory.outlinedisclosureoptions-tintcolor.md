

- UIKit
- UICellAccessory
- UICellAccessory.OutlineDisclosureOptions
-  tintColor 

Instance Property

# tintColor

The tint color to apply to the accessory.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var tintColor: UIColor?
```

## Discussion

The default value of this property is `nil`, which means that the accessory uses the system default tint color.

## See Also

### Accessing configuration options

var isHidden: Bool

A Boolean value that determines whether the cell hides the accessory.

var reservedLayoutWidth: UICellAccessory.LayoutDimension

The layout width that the system reserves for the accessory, and then centers the accessory within.

var style: UICellAccessory.OutlineDisclosureOptions.Style

The style of the outline disclosure accessory.

enum Style

Constants that describe the style of the outline disclosure accessory.

