

- SpriteKit
- SKTileMapNode
-  colorBlendFactor 

Instance Property

# colorBlendFactor

Controls the blending between the texture and the tile map object’s color. Values are clamped between zero and one where zero has no color blending and one has the maximum color blending.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**watchOS**

``` source
var colorBlendFactor: CGFloat { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var colorBlendFactor: CGFloat { get set }
```

## See Also

### Tinting a Tile Map

var color: UIColor

The base color for the tile map. The influence of the color over the tile map node’s textures is controlled by colorBlendFactor.

