

- UIKit
- UICellAccessory
- UICellAccessory.CustomViewConfiguration
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

let customView: UIView

The custom view to display for the accessory.

let placement: UICellAccessory.Placement

The placement for the accessory.

var reservedLayoutWidth: UICellAccessory.LayoutDimension

The layout width that the system reserves for the accessory, and then centers the accessory within.

var maintainsFixedSize: Bool

A Boolean value that determines whether to preserve the frame size of the custom view.

