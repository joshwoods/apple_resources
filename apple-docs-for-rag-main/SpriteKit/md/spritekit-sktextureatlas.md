

- SpriteKit
-  SKTextureAtlas 

Class

# SKTextureAtlas

A collection of textures optimized for storage and drawing performance.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SKTextureAtlas
```

## Mentioned in 

About Texture Atlases

Maximizing Texture Performance

Maximizing Node Drawing Performance

## Overview

An `SKTextureAtlas` is a collection of textures that were either created from an `.atlas` folder in the app bundle, or created at runtime. Texture atlases improve memory usage and rendering performance by reducing draw calls. Whenever you have textures that are always used together, store them in an atlas for best results.

SpriteKit implicitly loads an atlas when one of the atlas’s textures is accessed. Use textureNamed(_:) when you want to explicitly access a texture atlas’s contents.

The preferred place to create a texture atlas is within an asset catalog (see Creating a Sprite Atlas), but you can also put your source textures in an `.atlas` folder in the app bundle.

## Topics

### First Steps

About Texture Atlases

Learn about the benefits of having a texture atlas, and the process for using it.

### Accessing Textures

Retrieve textures from an atlas by the textures’ filenames.

func textureNamed(String) -> SKTexture

Creates a texture from data stored in the texture atlas.

### Creating a Texture Atlas Programmatically

Create an atlas in code.

convenience init(named: String)

Creates a texture atlas from data stored in the app bundle.

convenience init(dictionary: [String : Any])

Creates a texture atlas from a set of image files.

### Preloading Textures

Gain fine-tuned control over when an atlas is decoded.

func preload(completionHandler: () -> Void)

Loads an atlas object’s textures into memory, calling a completion handler after the task completes.

class func preloadTextureAtlases([SKTextureAtlas], withCompletionHandler: () -> Void)

Loads the textures of multiple atlas objects into memory, calling a completion handler after the task completes.

class func preloadTextureAtlasesNamed([String], withCompletionHandler: ((any Error)?, [SKTextureAtlas]) -> Void)

Loads the textures of multiple atlases into memory, calling a completion handler after the task completes.

### Reading Source Image Filenames

Determine whether an atlas contains a particular source image.

var textureNames: [String]

The names of the texture images stored in the atlas.

### Instance Properties

var customPlaygroundQuickLook: PlaygroundQuickLook

A custom playground quick look for this instance.

Deprecated

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Textures

Maximizing Texture Performance

Speed up image display and enable more images to be displayed at one time.

class SKTexture

An image, decoded on the GPU, that can be used to render various SpriteKit objects.

class SKMutableTexture

A texture whose contents can be dynamically updated.

