

- RealityKit
- TextureResource
-  replaceAsync(withImage:options:) Deprecated

Instance Method

# replaceAsync(withImage:options:)

Asynchronously replaces the texture with a Core Graphics image.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor @preconcurrency
func replaceAsync(
    withImage cgImage: CGImage,
    options: TextureResource.CreateOptions
) -> LoadRequest
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

### Deprecated

static func generate(from: CGImage, withName: String?, options: TextureResource.CreateOptions) throws -> TextureResource

Synchronously creates a texture resource from an in-memory Core Graphics image.

Deprecated

static func generateAsync(from: CGImage, withName: String?, options: TextureResource.CreateOptions) -> LoadRequest&lt;TextureResource>

Asynchronously generates a texture resource from an in-memory Core Graphics image.

Deprecated

static func generate(from: CGImage, named: String?, options: TextureResource.CreateOptions) async throws -> TextureResource

Asynchronously generates a texture resource from an in-memory Core Graphics image.

Deprecated

static func loadAsync(contentsOf: URL, withName: String?, options: TextureResource.CreateOptions) -> LoadRequest&lt;TextureResource>

Asynchronously loads a texture resource from a URL with options.

Deprecated

