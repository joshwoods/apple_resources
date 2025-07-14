

- UIKit
- UICellAccessory
- UICellAccessory.CustomViewConfiguration
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

let customView: UIView

The custom view to display for the accessory.

let placement: UICellAccessory.Placement

The placement for the accessory.

var reservedLayoutWidth: UICellAccessory.LayoutDimension

The layout width that the system reserves for the accessory, and then centers the accessory within.

var tintColor: UIColor?

The tint color to apply to the accessory.

var maintainsFixedSize: Bool

A Boolean value that determines whether to preserve the frame size of the custom view.

