

- UIKit
- UICellAccessory
- UICellAccessory.PopUpMenuOptions
-  reservedLayoutWidth 

Instance Property

# reservedLayoutWidth

The layout width that the system reserves for the accessory, and then centers the accessory within.

iOS 16.0+iPadOS 16.0+Mac CatalysttvOS 14.0+visionOS

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

