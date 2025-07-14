

- UIKit
-  UIPointerAccessory 

Class

# UIPointerAccessory

Constants that describe accessories to display alongside the primary pointer.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
class UIPointerAccessory
```

## Topics

### Creating a pointer accessory

convenience init(UIPointerShape, position: UIPointerAccessory.Position)

Creates a pointer accessory with the specified shape and position.

class func arrow(UIPointerAccessory.Position) -> Self

Creates a pointer accessory with an arrow shape at the specified position.

### Matching the angle

var orientationMatchesAngle: Bool

A Boolean value that indicates whether the system rotates the accessory to match its angle.

### Getting the shape

var shape: UIPointerShape

The shape of the accessory.

### Getting the position

var position: __UIPointerAccessoryPosition

The position of the accessory relative to the primary pointer.

struct Position

A structure that specifies the position of the accessory relative to the primary pointer.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Pointer styles

class UIPointerStyle

An object that defines the pointer shape and effect.

enum UIPointerShape

An object that defines the shape of custom pointers.

enum UIPointerEffect

An effect that alters a view’s appearance when a pointer enters the current region.

