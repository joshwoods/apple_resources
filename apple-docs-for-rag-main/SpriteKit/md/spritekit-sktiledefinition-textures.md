

- SpriteKit
- SKTileDefinition
-  textures 

Instance Property

# textures

An array of SKTexture objects that defines the tile definition object’s content.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var textures: [SKTexture] { get set }
```

## Discussion

If the tile is non-animated, this will be an array containing one textures.

## See Also

### Configure Animated Tile Properties

var normalTextures: [SKTexture]

An array of SKTexture objects used to generate the normals for the tile to simulate 3D lighting.

var timePerFrame: CGFloat

The duration, in seconds, that each texture in the textures array is displayed before switching to the next texture in the sequence.

