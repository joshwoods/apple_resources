

- UIKit
- UICellAccessory
- UICellAccessory.CustomViewConfiguration
-  maintainsFixedSize 

Instance Property

# maintainsFixedSize

A Boolean value that determines whether to preserve the frame size of the custom view.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var maintainsFixedSize: Bool
```

## Discussion

When the value of this property is true, the system preserves the current frame size of the view. When the value of this property is false, the system sizes the view during layout of the accessories.

The default value of this property is false.

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

var tintColor: UIColor?

The tint color to apply to the accessory.

