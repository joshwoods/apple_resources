

- UIKit
- UIPointerAccessory
- UIPointerAccessory.Position
-  angle 

Instance Property

# angle

The angle of the accessory’s position, measured in radians clockwise from the top of the primary pointer.

iOS 15.0+iPadOS 15.0+Mac CatalystvisionOS

``` source
var angle: CGFloat
```

## See Also

### Creating a custom accessory position

init(offset: CGFloat, angle: CGFloat)

Creates a custom accessory position with the specified offset and angle.

var offset: CGFloat

The offset of the accessory from the primary pointer.

static let defaultOffset: CGFloat

A constant that specifies the default offset of an accessory from the primary pointer shape.

