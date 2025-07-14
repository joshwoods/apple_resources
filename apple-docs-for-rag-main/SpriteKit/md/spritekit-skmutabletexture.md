

- SpriteKit
-  SKMutableTexture 

Class

# SKMutableTexture

A texture whose contents can be dynamically updated.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class SKMutableTexture
```

## Mentioned in 

Loading and Using Textures

## Overview

Normally, SpriteKit textures (SKTexture objects) are static, meaning that once created, their contents cannot be changed. This is important because a static image can be more efficiently managed inside the graphics hardware. However, sometimes you need to be able to update the contents of a texture dynamically. In this case, you should use a mutable texture. Because there is a performance penalty for updating the texture’s contents, consider other options first. For example, you can render a texture in hardware using the texture(from:) method and a node tree.

To use this class, create a mutable texture using either one of its creation methods or those of its superclass. Then, when you need to update the mutable texture object’s contents, call the modifyPixelData(_:) method. Your block is called with the location of the texture in memory. Your block should update this texture and then return.

## Topics

### Creating an Empty Mutable Texture

init(size: CGSize, pixelFormat: Int32)

Initializes an empty texture with a specific size and format.

init(size: CGSize)

Initializes an empty texture with a specific size.

### Modifying a Mutable Texture’s Contents

func modifyPixelData((UnsafeMutableRawPointer?, Int) -> Void)

Modifies the contents of a mutable texture.

## Relationships

### Inherits From

- SKTexture

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

### Textures

Maximizing Texture Performance

Speed up image display and enable more images to be displayed at one time.

class SKTexture

An image, decoded on the GPU, that can be used to render various SpriteKit objects.

class SKTextureAtlas

A collection of textures optimized for storage and drawing performance.

