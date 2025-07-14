

- SpriteKit
-  SKTileDefinition 

Class

# SKTileDefinition

A single tile that can be repeated in a tile map.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class SKTileDefinition
```

## Overview

To define the visual representation of a single tile, you create an SKTileDefinition object with texture and size information. Tile definitions support separate normal textures, for simulating 3D lighting, and arrays of textures for animation with speed controlled by the timePerFrame property. Textures can be rotated in 90˚ increments or flipped either vertically or horizontally.

Once a tile definition has been created, you encapsulate it in a SKTileGroup which is added to a SKTileSet which, in turn, is displayed in the scene with a SKTileMapNode.

## Topics

### Creating a Tile with a Texture

init(texture: SKTexture)

Initializes a new tile definition with a single texture.

### Creating a Tile with a Normal Texture

Create a tile with an additional texture that’s used for lighting effects.

init(texture: SKTexture, normalTexture: SKTexture, size: CGSize)

Initializes a new tile definition with a single texture and separate normal texture for simulating 3D lighting.

### Creating a Tile with a Size

init(texture: SKTexture, size: CGSize)

Initializes a new tile definition of a specified size with a single texture.

### Creating an Animated Tile

Create an animated Tile by passing in an array of textures (animation frames) and their respective times per frame.

init(textures: [SKTexture], normalTextures: [SKTexture], size: CGSize, timePerFrame: CGFloat)

Initializes a new tile definition with arrays of textures and normal textures for animation.

init(textures: [SKTexture], size: CGSize, timePerFrame: CGFloat)

Initializes a new tile definition with an array of textures for animation.

### Flipping a Tile Vertically or Horizontally

var flipHorizontally: Bool

A Boolean that flips the definition’s image vertically.

var flipVertically: Bool

A Boolean that flips the definition’s image horizontally.

### Rotating a Tile

var rotation: SKTileDefinitionRotation

The rotation of the tile definition in 90˚ increments.

enum SKTileDefinitionRotation

The allowed rotations for a given tile.

### Configure Animated Tile Properties

var textures: [SKTexture]

An array of SKTexture objects that defines the tile definition object’s content.

var normalTextures: [SKTexture]

An array of SKTexture objects used to generate the normals for the tile to simulate 3D lighting.

var timePerFrame: CGFloat

The duration, in seconds, that each texture in the textures array is displayed before switching to the next texture in the sequence.

### Reading or Adding a Tile’s Custom Data

var userData: NSMutableDictionary?

A dictionary containing arbitrary data.

### Reading or Adjusting a Tile’s Instance Properties

var name: String?

A name associated with the tile definition.

var placementWeight: Int

The placement weight of the tile definition.

var size: CGSize

The size of the tile definition in points.

## Relationships

### Inherits From

- NSObject

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

## See Also

### Tiling

class SKTileMapNode

A two-dimensional array of images.

class SKTileGroup

A set of tiles that collectively define one type of terrain.

class SKTileGroupRule

Rules that describe how various tiles should be placed in a map.

class SKTileSet

A container for related tile groups.

