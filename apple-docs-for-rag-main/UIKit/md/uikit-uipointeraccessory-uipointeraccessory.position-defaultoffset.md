

- UIKit
- UIPointerAccessory
- UIPointerAccessory.Position
-  defaultOffset 

Type Property

# defaultOffset

A constant that specifies the default offset of an accessory from the primary pointer shape.

iOS 15.0+iPadOS 15.0+Mac CatalystvisionOS

``` source
static let defaultOffset: CGFloat
```

## See Also

### Creating a custom accessory position

init(offset: CGFloat, angle: CGFloat)

Creates a custom accessory position with the specified offset and angle.

var angle: CGFloat

The angle of the accessory’s position, measured in radians clockwise from the top of the primary pointer.

var offset: CGFloat

The offset of the accessory from the primary pointer.

