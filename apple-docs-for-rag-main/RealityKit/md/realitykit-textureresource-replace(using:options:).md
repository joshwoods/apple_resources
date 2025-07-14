

- RealityKit
- TextureResource
-  replace(using:options:) 

Instance Method

# replace(using:options:)

Asynchronously replaces the texture with a Core Graphics image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func replace(
    using cgImage: CGImage,
    options: TextureResource.CreateOptions
) async throws
```

## Parameters 

`cgImage`  

The source image.

`options`  

Options that specify the type of texture to create. To preserve `TextureResource` usage, specify the same semantic.

## Discussion

Don’t use this method for updates at frame-rate frequency. For frequent texture changes, see replace(withDrawables:). To ensure consistent usage of this texture resource, pass the same semantic in `options` that you use to create the resource.

Note

The contents of a modified texture resource don’t sync between network clients.

## See Also

### Modifying the texture

func replace(withDrawables: TextureResource.DrawableQueue)

Dynamically replaces the texture with a drawable queue.

func replace(withImage: CGImage, options: TextureResource.CreateOptions) throws

Dynamically replaces the texture with a Core Graphics image.

func replace(with: LowLevelTexture)

Replaces a texture resource with a low-level texture.

