

- RealityKit
- TextureResource
-  generate(from:named:options:) Deprecated

Type Method

# generate(from:named:options:)

Asynchronously generates a texture resource from an in-memory Core Graphics image.

visionOS 1.0–2.0Deprecated

``` source
@MainActor @preconcurrency
static func generate(
    from cgImage: CGImage,
    named resourceName: String? = nil,
    options: TextureResource.CreateOptions
) async throws -> TextureResource
```

## Parameters 

`cgImage`  

The source image.

`resourceName`  

A unique name for syncing the texture resource across the network. The name is empty if you don’t include one.

`options`  

A configuration for generating the texture.

## Return Value

A texture resource.

## Discussion

This method creates a texture resource from an existing CGImage with specific options. RealityKit uses the resource name to identify resources, and to match texture resources between networked peers. Specify a unique name for each texture resource you load or generate.

## See Also

### Deprecated

static func generate(from: CGImage, withName: String?, options: TextureResource.CreateOptions) throws -> TextureResource

Synchronously creates a texture resource from an in-memory Core Graphics image.

Deprecated

static func generateAsync(from: CGImage, withName: String?, options: TextureResource.CreateOptions) -> LoadRequest&lt;TextureResource>

Asynchronously generates a texture resource from an in-memory Core Graphics image.

Deprecated

func replaceAsync(withImage: CGImage, options: TextureResource.CreateOptions) -> LoadRequest&lt;TextureResource>

Asynchronously replaces the texture with a Core Graphics image.

Deprecated

static func loadAsync(contentsOf: URL, withName: String?, options: TextureResource.CreateOptions) -> LoadRequest&lt;TextureResource>

Asynchronously loads a texture resource from a URL with options.

Deprecated

