

- RealityKit
- TextureResource
-  loadAsync(contentsOf:withName:) Deprecated

Type Method

# loadAsync(contentsOf:withName:)

Asynchronously loads a texture resource from a URL.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 10.15–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor @preconcurrency
static func loadAsync(
    contentsOf url: URL,
    withName resourceName: String? = nil
) -> LoadRequest
```

## Parameters 

`url`  

The path or address of the file to load.

`resourceName`  

A unique name the method assigns to the resource it loads, for use in network synchronization.

## Return Value

A load operation that publishes the resource.

## Discussion

RealityKit uses the resource name to distinguish resources locally, and to match texture resources between networked peers. Specify a unique name for each texture resource you load or generate.

## See Also

### Loading a texture

convenience init(named: String, in: Bundle?) async throws

Asynchronously loads a texture resource from a bundle.

convenience init(named: String, in: Bundle?, options: TextureResource.CreateOptions) async throws

Asynchronously loads a texture resource from a bundle with options.

convenience init(contentsOf: URL, withName: String?, options: TextureResource.CreateOptions) async throws

Asynchronously creates a texture resource from a file URL with creation options.

convenience init(contentsOf: URL, withName: String?) async throws

Synchronously creates a texture resource from a file URL.

static func load(named: String, in: Bundle?) throws -> TextureResource

Returns a texture resource by synchronously loading it from a bundle.

static func load(named: String, in: Bundle?, options: TextureResource.CreateOptions) throws -> TextureResource

Returns a texture resource by synchronously loading it from a bundle with options.

static func load(contentsOf: URL, withName: String?, options: TextureResource.CreateOptions) throws -> TextureResource

Synchronously loads a texture resource from a URL with options.

static func load(contentsOf: URL, withName: String?) throws -> TextureResource

Synchronously loads a texture resource from a URL.

static func loadAsync(named: String, in: Bundle?) -> LoadRequest&lt;TextureResource>

Returns a load request that creates a texture resource by asynchronously loading it from a bundle.

Deprecated

static func loadAsync(named: String, in: Bundle?, options: TextureResource.CreateOptions) -> LoadRequest&lt;TextureResource>

Returns a load request that creates a texture resource by asynchronously loading it from a bundle with options.

Deprecated

