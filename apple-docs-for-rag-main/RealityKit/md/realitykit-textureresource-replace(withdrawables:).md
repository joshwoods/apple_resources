

- RealityKit
- TextureResource
-  replace(withDrawables:) 

Instance Method

# replace(withDrawables:)

Dynamically replaces the texture with a drawable queue.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
func replace(withDrawables drawableQueue: TextureResource.DrawableQueue)
```

## See Also

### Modifying the texture

func replace(withImage: CGImage, options: TextureResource.CreateOptions) throws

Dynamically replaces the texture with a Core Graphics image.

func replace(using: CGImage, options: TextureResource.CreateOptions) async throws

Asynchronously replaces the texture with a Core Graphics image.

func replace(with: LowLevelTexture)

Replaces a texture resource with a low-level texture.

