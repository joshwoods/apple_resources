

- SpriteKit
- SKFieldNode
-  minimumRadius 

Instance Property

# minimumRadius

The minimum value for distance-based effects.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var minimumRadius: Float { get set }
```

**watchOS**

``` source
var minimumRadius: Float { get set }
```

## Discussion

When the distance between the node and a physics body is calculated, any distance shorter than the value stored in the minimumRadius property is treated as if it is equal to it. The default value is a very small (but nonzero) value.

## See Also

### Determining Which Physics Bodies Are Affected by the Field

var isEnabled: Bool

A Boolean value that indicates whether the field is active.

var isExclusive: Bool

A Boolean value that indicates whether the field node should override all other field nodes that might otherwise affect physics bodies.

var region: SKRegion?

The area (relative to the node’s origin) that the field affects.

var categoryBitMask: UInt32

A mask that defines which categories this field belongs to.

