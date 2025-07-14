

- RealityKit
- TextureResource
-  replace(with:) 

Instance Method

# replace(with:)

Replaces a texture resource with a low-level texture.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
func replace(with texture: LowLevelTexture)
```

## Parameters 

`texture`  

The texture data that defines the resource.

## Discussion

Warning

It’s more efficient to use replace(using:) to update a LowLevelTexture on the GPU than it is to update the `TextureResource`. Prefer to update the `LowLevelTexture` directly instead.

## See Also

### Modifying the texture

func replace(withDrawables: TextureResource.DrawableQueue)

Dynamically replaces the texture with a drawable queue.

func replace(withImage: CGImage, options: TextureResource.CreateOptions) throws

Dynamically replaces the texture with a Core Graphics image.

func replace(using: CGImage, options: TextureResource.CreateOptions) async throws

Asynchronously replaces the texture with a Core Graphics image.

