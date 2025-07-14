

- UIKit
- UIPointerAccessory
- UIPointerAccessory.Position
-  init(offset:angle:) 

Initializer

# init(offset:angle:)

Creates a custom accessory position with the specified offset and angle.

iOS 15.0+iPadOS 15.0+Mac CatalystvisionOS

``` source
init(
    offset: CGFloat = Position.defaultOffset,
    angle: CGFloat = 0
)
```

## See Also

### Creating a custom accessory position

var angle: CGFloat

The angle of the accessory’s position, measured in radians clockwise from the top of the primary pointer.

var offset: CGFloat

The offset of the accessory from the primary pointer.

static let defaultOffset: CGFloat

A constant that specifies the default offset of an accessory from the primary pointer shape.

