

- SpriteKit
- SKFieldNode
-  isExclusive 

Instance Property

# isExclusive

A Boolean value that indicates whether the field node should override all other field nodes that might otherwise affect physics bodies.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**watchOS**

``` source
var isExclusive: Bool { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var isExclusive: Bool { get set }
```

## Discussion

If the value is set to true and a physics body is within this field’s region, all other field nodes that might otherwise affect this body are ignored. The default value is false.

If you set this property to true on multiple field nodes within a scene, their regions should not overlap. If they do, the results are undefined.

## See Also

### Determining Which Physics Bodies Are Affected by the Field

var isEnabled: Bool

A Boolean value that indicates whether the field is active.

var region: SKRegion?

The area (relative to the node’s origin) that the field affects.

var minimumRadius: Float

The minimum value for distance-based effects.

var categoryBitMask: UInt32

A mask that defines which categories this field belongs to.

