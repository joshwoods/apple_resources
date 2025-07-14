

- UIKit
-  UIDynamicItemCollisionBoundsType 

Enumeration

# UIDynamicItemCollisionBoundsType

Constants that indicate the shape of the item’s collision bounds.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
enum UIDynamicItemCollisionBoundsType
```

## Topics

### Constants

case rectangle

Rectangular collision bounds.

case ellipse

Elliptical collision bounds. The shape of the ellipse is determined by the width and height of the item’s bounds property.

case path

Path-based collision bounds. For this type, the shape is a UIBezierPath object stored in the item’s collisionBoundingPath property. See the description of that property for information about how to configure the path itself.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

