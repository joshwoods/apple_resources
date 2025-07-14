

- SpriteKit
- SKTexture
-  Texture Initializers 

API Collection

# Texture Initializers

See the various ways to create and use textures in SpriteKit.

## Overview

Use these functions to create a new texture. While doing so, you should be aware of the memory implications of texture memory, and the other ways to get textures other than `SKTexture` initializers.

### Memory Considerations

When creating textures you should be aware of the memory consumed as a result of their file size dimensions. Often, the memory available to prepared textures is limited by hardware because textures are loaded in VRAM. Consider the following tips:

- Access a texture only when needed and dispose of it when you are done. This frees up memory for other parts of the app.

- Avoid loading too many textures in a single pass through the rendering loop. The process of decoding an image from disk is an expensive one and can therefore cause a few frames to be skipped. To avoid performance hiccups, preload textures ahead of time, such as when the scene is loaded.

- If you frequently use that same textures together (for example, all the grass tiles any time grass is displayed in a scene) then you should consider bundling them into an SKTextureAtlas to increase loading and runtime peformance.

### Ways to Access Textures

In addition to the Texture Initializers in `SKTexture`, the following other classes vend textures, too:

- Access a texture by its original filename within a SpriteKit texture atlas folder using `SKTextureAtlas`’s textureNamed(_:)

- Create a texture by rendering an existing node in the tree, including its children, using `SKView`’s texture(from:)

## Topics

### Filename Initializer

Search the app bundle for an image by filename.

convenience init(imageNamed: String)

Create a new texture object from an image file stored in the app bundle.

### Texture Within a Texture

convenience init(rect: CGRect, in: SKTexture)

Creates a new texture from a sub-rectangle of an existing texture.

### Texture from Image

convenience init(image: UIImage)

Create a new texture object from an image object.

convenience init(cgImage: CGImage)

Create a new texture object from a Quartz 2D image.

### Texture with Effects

func applying(CIFilter) -> Self

Creates a new texture by applying a Core Image filter to an existing texture.

### Texture from Data

convenience init(data: Data, size: CGSize)

Creates a new texture from raw pixel data.

convenience init(data: Data, size: CGSize, rowLength: UInt32, alignment: UInt32)

Creates a new texture from custom formatted raw pixel data.

convenience init(data: Data, size: CGSize, flipped: Bool)

Creates a new texture from raw pixel data.

### Texture from Normal Map

func generatingNormalMap() -> Self

Creates a normal map texture by analyzing the contents of an existing texture.

func generatingNormalMap(withSmoothness: CGFloat, contrast: CGFloat) -> Self

Creates a normal map texture by analyzing the contents of an existing texture.

### Noise Textures

convenience init(vectorNoiseWithSmoothness: CGFloat, size: CGSize)

Creates a new texture whose contents are procedurally generated directional noise data.

convenience init(noiseWithSmoothness: CGFloat, size: CGSize, grayscale: Bool)

Creates a new texture whose contents are procedurally generated color noise data.

### Texture from Noise Map

convenience init(noiseMap: GKNoiseMap)

Creates a texture from the specified noise map.

## See Also

### First Steps

Loading and Using Textures

Learn the basics about using textures in SpriteKit.

