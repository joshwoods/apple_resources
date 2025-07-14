

- SpriteKit
- SKTileDefinition
-  normalTextures 

Instance Property

# normalTextures

An array of SKTexture objects used to generate the normals for the tile to simulate 3D lighting.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var normalTextures: [SKTexture] { get set }
```

## Discussion

If the tile is non-animated, this will be an array containing one texture.

## See Also

### Configure Animated Tile Properties

var textures: [SKTexture]

An array of SKTexture objects that defines the tile definition object’s content.

var timePerFrame: CGFloat

The duration, in seconds, that each texture in the textures array is displayed before switching to the next texture in the sequence.

