

- RealityKit
- TextureResource
-  replace(withImage:options:) 

Instance Method

# replace(withImage:options:)

Dynamically replaces the texture with a Core Graphics image.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
func replace(
    withImage cgImage: CGImage,
    options: TextureResource.CreateOptions
) throws
```

## Parameters 

`cgImage`  

The source image.

`options`  

Options that specify the type of texture to create.

## Discussion

This method blocks until the resource updates. Don’t use this method for updates at frame-rate frequency. For frequent texture changes, see replace(withDrawables:). If you have an attached TextureResource.DrawableQueue on this resource, this function detaches it.

To ensure consistent usage of this texture resource, pass the same semantic in `options` that you use to create the resource.

Note

The contents of a modified texture resource don’t sync between network clients.

## See Also

### Modifying the texture

func replace(withDrawables: TextureResource.DrawableQueue)

Dynamically replaces the texture with a drawable queue.

func replace(using: CGImage, options: TextureResource.CreateOptions) async throws

Asynchronously replaces the texture with a Core Graphics image.

func replace(with: LowLevelTexture)

Replaces a texture resource with a low-level texture.

