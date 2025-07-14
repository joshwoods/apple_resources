

- RealityKit
- TextureResource
-  loadAsync(contentsOf:withName:options:) Deprecated

Type Method

# loadAsync(contentsOf:withName:options:)

Asynchronously loads a texture resource from a URL with options.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor @preconcurrency
static func loadAsync(
    contentsOf url: URL,
    withName resourceName: String? = nil,
    options: TextureResource.CreateOptions
) -> LoadRequest
```

## Parameters 

`url`  

The path or address of the file to load.

`resourceName`  

A unique name the method assigns to the resource it loads, for use in network synchronization.

`options`  

A configuration for generating the texture.

## Return Value

A load operation that publishes the resource.

## Discussion

RealityKit uses the resource name to distinguish resources locally, and to match texture resources between networked peers. Specify a unique name for each texture resource you load or generate.

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

static func generate(from: CGImage, named: String?, options: TextureResource.CreateOptions) async throws -> TextureResource

Asynchronously generates a texture resource from an in-memory Core Graphics image.

Deprecated

