

- UIKit
- UICellAccessory
-  UICellAccessory.CustomViewConfiguration 

Structure

# UICellAccessory.CustomViewConfiguration

Configuration options for a custom accessory.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
struct CustomViewConfiguration
```

## Topics

### Creating configuration options

init(customView: UIView, placement: UICellAccessory.Placement, isHidden: Bool?, reservedLayoutWidth: UICellAccessory.LayoutDimension?, tintColor: UIColor?, maintainsFixedSize: Bool?)

Creates a custom accessory options structure.

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

var maintainsFixedSize: Bool

A Boolean value that determines whether to preserve the frame size of the custom view.

## See Also

### Creating a custom accessory

static func customView(configuration: UICellAccessory.CustomViewConfiguration) -> UICellAccessory

Creates a custom view accessory.

