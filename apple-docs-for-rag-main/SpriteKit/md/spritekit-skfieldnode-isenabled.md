

- SpriteKit
- SKFieldNode
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that indicates whether the field is active.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var isEnabled: Bool { get set }
```

**watchOS**

``` source
var isEnabled: Bool { get set }
```

## Mentioned in 

Adding Physics Fields to a Scene

## See Also

### Determining Which Physics Bodies Are Affected by the Field

var isExclusive: Bool

A Boolean value that indicates whether the field node should override all other field nodes that might otherwise affect physics bodies.

var region: SKRegion?

The area (relative to the node’s origin) that the field affects.

var minimumRadius: Float

The minimum value for distance-based effects.

var categoryBitMask: UInt32

A mask that defines which categories this field belongs to.

