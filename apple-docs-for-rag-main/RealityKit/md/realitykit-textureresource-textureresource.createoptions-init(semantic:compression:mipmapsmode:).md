

- RealityKit
- TextureResource
- TextureResource.CreateOptions
-  init(semantic:compression:mipmapsMode:) 

Initializer

# init(semantic:compression:mipmapsMode:)

Creates a texture creation options structure.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    semantic: TextureResource.Semantic?,
    compression: TextureResource.Compression,
    mipmapsMode: TextureResource.MipmapsMode = .allocateAndGenerateAll
)
```

## Parameters 

`semantic`  

The intended use of the texture resource.

`compression`  

Compression to be applied to the texture.

`mipmapsMode`  

Whether to automatically allocate or generate mipmaps.

## Discussion

The `semantic` value you pass tells RealityKit how you plan to use the texture data from this resource. For example, passing TextureResource.Semantic.color lets RealityKit know you’re using the texture to pass perceptual color information to the shaders, such as for providing a UV-mapped base color for physically based rendering materials. Passing TextureResource.Semantic.raw tells RealityKit to pass the pixel values with as little processing as possible.

If semantic is `nil`, RealityKit tries to infer a semantic from the texture’s source data. If it’s unable to determine a semantic from the texture source data, it will infer a semantic from the texture’s usage. Providing a value for `semantic` ensures that RealityKit passes the texture resource exactly as you intend.

Note

RealityKit only takes embedded color space data into account when rendering a texture if you pass TextureResource.Semantic.color for `semantic`.

