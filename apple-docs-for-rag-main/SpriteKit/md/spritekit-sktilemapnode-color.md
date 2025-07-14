

- SpriteKit
- SKTileMapNode
-  color 

Instance Property

# color

The base color for the tile map. The influence of the color over the tile map node’s textures is controlled by colorBlendFactor.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
var color: UIColor { get set }
```

**macOS**

``` source
@MainActor
var color: NSColor { get set }
```

**watchOS**

``` source
var color: UIColor { get set }
```

## See Also

### Tinting a Tile Map

var colorBlendFactor: CGFloat

Controls the blending between the texture and the tile map object’s color. Values are clamped between zero and one where zero has no color blending and one has the maximum color blending.

