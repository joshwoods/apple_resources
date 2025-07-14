

- SpriteKit
- SKFieldNode
-  categoryBitMask 

Instance Property

# categoryBitMask

A mask that defines which categories this field belongs to.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var categoryBitMask: UInt32 { get set }
```

**watchOS**

``` source
var categoryBitMask: UInt32 { get set }
```

## Discussion

Every field in a scene can be assigned to up to 32 different categories, each corresponding to a bit in the bit mask. The mask values are not predetermined by Sprite Kit. You define the mask values that are used in your game. The field node’s categoryBitMask property is compared to a physics body’s fieldBitMask property using a logical AND operation. If the result is nonzero, the field is applied to the physics body.

The default value is `0xFFFFFFFF` (all bits set).

## See Also

### Determining Which Physics Bodies Are Affected by the Field

var isEnabled: Bool

A Boolean value that indicates whether the field is active.

var isExclusive: Bool

A Boolean value that indicates whether the field node should override all other field nodes that might otherwise affect physics bodies.

var region: SKRegion?

The area (relative to the node’s origin) that the field affects.

var minimumRadius: Float

The minimum value for distance-based effects.

