

- SpriteKit
- SKLightNode
-  categoryBitMask 

Instance Property

# categoryBitMask

A mask that defines which categories this light belongs to.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**watchOS**

``` source
var categoryBitMask: UInt32 { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var categoryBitMask: UInt32 { get set }
```

## Mentioned in 

Lighting a Sprite with Light Nodes

## Discussion

Every light in a scene can be assigned to up to 32 different categories, each corresponding to a bit in the bit mask. SpriteKit does not predefine any lighting categories, so it is up to you to define which values are used in your game. When a scene is rendered, a light’s categoryBitMask property is compared to each sprite node’s lightingBitMask, shadowCastBitMask, and shadowedBitMask properties to determine whether that sprite interacts with the light.

The default value is `0x00000001`.

## See Also

### Determining Whether a Light Node Is Active

var isEnabled: Bool

A Boolean value that indicates whether the node is casting light.

