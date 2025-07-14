

- SpriteKit
-  SKTileMapNode 

Class

# SKTileMapNode

A two-dimensional array of images.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**watchOS**

``` source
class SKTileMapNode
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
class SKTileMapNode
```

## Overview

`SKTileMapNode` does the work of laying out predefined tiles in a grid of any size. Typically, you configure 9-slice images (tile groups) in Xcode’s SpriteKit scene editor and paint the look of your tile map ahead of time versus configuring the tile map in code.

As with sprite nodes, you can layer tile maps with different blend modes or control it with actions and physics, for example, for the purpose of parallax scrolling. The rendered tile map can be post processed with an SKShader to add effects such as motion blur or atmospheric perspective.

Note

A tile map can only render tile definitions that exist within the SKTileSet you have provided it.

Important

A tile map does not expose its tiles as nodes, and therefore you cannot assign individual tiles with a different zPosition or physicsBody. Instead, layer tile map nodes on top of each other at the varying zPositions, and layer invisible `SKNodes` on top of the tile map node to attach physicsBodies to your tile map node.

To work with a tile map programmatically, you supply `SKTileMapNode` with a tile set that defines the tile definitions it can render. Then, fill each tile in the tile map with the fill(with:) method and set individual tiles with setTileGroup(_:andTileDefinition:forColumn:row:).

## Topics

### Creating a Tile Map Programmatically

Create a tile map manually instead of loading it from an archived `.sks` file.

Creating a Tile Map Programmatically

### Controlling a Tile Map’s On-Screen Position Relative to its Origin

var anchorPoint: CGPoint

Defines the point in the tile map that corresponds to its position.

### Reading or Manually Configuring the Tile Map’s Size

var tileSize: CGSize

The size of each tile in points.

var tileSet: SKTileSet

The tile set being used by this tile map. The tile map object can only display tiles that exist in this set.

var numberOfColumns: Int

The number of columns in the tile map

var numberOfRows: Int

The number of rows in the tile map.

### Querying the Tile Map’s Properties

func centerOfTile(atColumn: Int, row: Int) -> CGPoint

func tileColumnIndex(fromPosition: CGPoint) -> Int

func tileDefinition(atColumn: Int, row: Int) -> SKTileDefinition?

func tileGroup(atColumn: Int, row: Int) -> SKTileGroup?

func tileRowIndex(fromPosition: CGPoint) -> Int

Returns the tile map node object’s tile row index for the specified position in points.

var mapSize: CGSize

The overall size of the tile map.

### Tinting a Tile Map

var color: UIColor

The base color for the tile map. The influence of the color over the tile map node’s textures is controlled by colorBlendFactor.

var colorBlendFactor: CGFloat

Controls the blending between the texture and the tile map object’s color. Values are clamped between zero and one where zero has no color blending and one has the maximum color blending.

### Lighting a Tile Map

Configure how a sprite is lit when its near a light node.

var lightingBitMask: UInt32

A mask that defines how the tile map is lit by light nodes in the scene.

### Configuring How Alpha Values Blend the Sprite

Change how a sprite uses its alpha value, such as additive blending, that results in the sprite being brighter than it was before.

var blendMode: SKBlendMode

Defines the blend mode to use when compositing the tile map over other nodes.

### Working with Custom Shaders

var shader: SKShader?

Defines a shader which is applied to each tile of the tile map.

var attributeValues: [String : SKAttributeValue]

The values of each attribute associated with the node’s attached shader.

func setValue(SKAttributeValue, forAttribute: String)

Sets an attribute value for an attached shader.

func value(forAttributeNamed: String) -> SKAttributeValue?

The value of a shader attribute.

## Relationships

### Inherits From

- SKNode

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- Sendable
- UIActivityItemsConfigurationProviding
- UICoordinateSpace
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIUserActivityRestoring

## See Also

### Tiling

class SKTileDefinition

A single tile that can be repeated in a tile map.

class SKTileGroup

A set of tiles that collectively define one type of terrain.

class SKTileGroupRule

Rules that describe how various tiles should be placed in a map.

class SKTileSet

A container for related tile groups.

