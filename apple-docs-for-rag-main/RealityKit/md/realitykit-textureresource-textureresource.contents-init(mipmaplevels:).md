

- RealityKit
- TextureResource
- TextureResource.Contents
-  init(mipmapLevels:) 

Initializer

# init(mipmapLevels:)

Creates a texture contents object from an array of mipmaps.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
init(mipmapLevels: [TextureResource.Contents.MipmapLevel])
```

## Parameters 

`mipmapLevels`  

Pixel data for each mipmap level, starting with mipmap level `0`. Supply at least one mipmap level.

## Discussion

Note

Creating 3D textures requires you to build `MipmapLevel` with `mip()` methods that have a `bytesPerImage` parameter.

