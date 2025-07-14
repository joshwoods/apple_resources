

- SpriteKit
-  SKTexture 

Class

# SKTexture

An image, decoded on the GPU, that can be used to render various SpriteKit objects.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SKTexture
```

## Mentioned in 

Loading and Using Textures

Getting Started with Sprite Nodes

Preloading Textures into Memory

Maximizing Node Drawing Performance

About Texture Atlases

## Overview

An SKTexture object is an image that can be applied to SKSpriteNode and SKShapeNode objects, particles created by an SKEmitterNode object, or tiles used in an SKTileMapNode. A texture object manages the texture data and graphics resources that are needed to render the image. Most texture objects are created from source images stored in your app bundle—your game’s artwork. Once created, a texture object’s contents are immutable. Multiple sprites can share the same texture object, sharing a single resource.

### Deallocating a Texture

After a texture is loaded into the graphics hardware memory, it stays in memory until the referencing SKTexture object is deleted. This means that between levels (or in a dynamic game), you may need to make sure a texture object is deleted. Delete a SKTexture object by removing any strong references to it, including:

- All texture references from SKSpriteNode and SKEffectNode objects in your game

- Any strong references to the texture in your own code

- An SKTextureAtlas object that was used to create the texture object

## Topics

### First Steps

Create texture objects from images on disk or in memory.

Loading and Using Textures

Learn the basics about using textures in SpriteKit.

Texture Initializers

See the various ways to create and use textures in SpriteKit.

### Reading a Texture’s Size and Optional Source Location

Read the texture’s size or optional cropping rectangle.

func size() -> CGSize

Gets the size of the texture.

func textureRect() -> CGRect

Gets a rectangle that defines the portion of the texture used to render its image.

### Configuring a Texture’s Behavior for Scaling

Define the texture’s behavior at different scales.

var filteringMode: SKTextureFilteringMode

The filtering mode used when the size of a sprite drawn with the texture is not drawn at the texture’s native size.

enum SKTextureFilteringMode

Texture filtering modes to use when the texture is drawn in a size other than its native size.

var usesMipmaps: Bool

A Boolean value that indicates whether the texture attempts to generate mipmaps.

### Getting a Texture’s Underlying Image

func cgImage() -> CGImage

Returns the texture’s image data as a Quartz 2D image.

### Preloading a Texture for Performance

Gain fine-tuned control over when a texture is decoded.

Preloading Textures into Memory

Decompress images ahead of time to avoid performance issues during gameplay.

func preload(completionHandler: () -> Void)

Load texture data into memory, calling a completion handler after the task completes.

class func preload([SKTexture], withCompletionHandler: () -> Void)

Load the data of multiple textures into memory.

### Instance Properties

var customPlaygroundQuickLook: PlaygroundQuickLookDeprecated

## Relationships

### Inherits From

- NSObject

### Inherited By

- SKMutableTexture

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Textures

Maximizing Texture Performance

Speed up image display and enable more images to be displayed at one time.

class SKTextureAtlas

A collection of textures optimized for storage and drawing performance.

class SKMutableTexture

A texture whose contents can be dynamically updated.

