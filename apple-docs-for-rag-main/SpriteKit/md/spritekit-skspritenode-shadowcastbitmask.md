

- SpriteKit
- SKSpriteNode
-  shadowCastBitMask 

Instance Property

# shadowCastBitMask

A mask that defines which lights are occluded by this sprite.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**watchOS**

``` source
var shadowCastBitMask: UInt32 { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var shadowCastBitMask: UInt32 { get set }
```

## Mentioned in 

Lighting a Sprite with Light Nodes

## Discussion

To determine whether this sprite blocks the light (casting a shadow), the sprite’s shadowedBitMask property is tested against the light’s categoryBitMask property by performing a logical AND operation. If the comparison results in a nonzero value, the sprite casts a shadow past itself.

## See Also

### Lighting a Sprite

Lighting a Sprite with Light Nodes

Add lighting and shadows to your scene with light nodes.

var lightingBitMask: UInt32

A mask that defines how this sprite is lit by light nodes in the scene.

var shadowedBitMask: UInt32

A mask that defines which lights add shadows to the sprite.

var normalTexture: SKTexture?

A texture that specifies the normal map for the sprite.

