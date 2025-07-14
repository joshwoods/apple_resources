

- UIKit
- UIPointerAccessory
-  UIPointerAccessory.Position 

Structure

# UIPointerAccessory.Position

A structure that specifies the position of the accessory relative to the primary pointer.

iOS 15.0+iPadOS 15.0+Mac CatalystvisionOS

``` source
struct Position
```

## Topics

### Getting an accessory position

static var top: UIPointerAccessory.Position

An accessory position at the top of the primary pointer.

static var topRight: UIPointerAccessory.Position

An accessory position at the top-right of the primary pointer.

static var right: UIPointerAccessory.Position

An accessory position at the right of the primary pointer.

static var bottomRight: UIPointerAccessory.Position

An accessory position at the bottom-right of the primary pointer.

static var bottom: UIPointerAccessory.Position

An accessory position at the bottom of the primary pointer.

static var bottomLeft: UIPointerAccessory.Position

An accessory position at the bottom-left of the primary pointer.

static var left: UIPointerAccessory.Position

An accessory position at the left of the primary pointer.

static var topLeft: UIPointerAccessory.Position

An accessory position at the top-left of the primary pointer.

### Creating a custom accessory position

init(offset: CGFloat, angle: CGFloat)

Creates a custom accessory position with the specified offset and angle.

var angle: CGFloat

The angle of the accessory’s position, measured in radians clockwise from the top of the primary pointer.

var offset: CGFloat

The offset of the accessory from the primary pointer.

static let defaultOffset: CGFloat

A constant that specifies the default offset of an accessory from the primary pointer shape.

## Relationships

### Conforms To

- Sendable

## See Also

### Getting the position

var position: __UIPointerAccessoryPosition

The position of the accessory relative to the primary pointer.

