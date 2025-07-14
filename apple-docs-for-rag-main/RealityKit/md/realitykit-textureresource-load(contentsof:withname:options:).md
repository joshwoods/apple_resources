

- RealityKit
- TextureResource
-  load(contentsOf:withName:options:) 

Type Method

# load(contentsOf:withName:options:)

Synchronously loads a texture resource from a URL with options.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
static func load(
    contentsOf url: URL,
    withName resourceName: String? = nil,
    options: TextureResource.CreateOptions
) throws -> TextureResource
```

## Parameters 

`url`  

The URL of the resource.

`resourceName`  

A unique name the method assigns to the resource it loads, for use in network synchronization.

`options`  

A configuration for generating the texture.

## Return Value

The loaded resource.

## Discussion

Loading a TextureResource with this method blocks the main actor because it’s synchronous, so only call it from a command-line application. The method can stall a regular app, which makes it visibly hitch, and the system terminates an app if its UI becomes unresponsive. See init(named:in:) for an example that demonstrates how to safely load content.

This method loads the image that the `URL` specifies, and creates a texture resource from it. The method blocks until it finishes loading the image and creating the texture resource.

RealityKit uses the resource name to identify resources, and to match texture resources between networked peers. Specify a unique name for each texture resource you load or generate.

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

static func load(contentsOf: URL, withName: String?) throws -> TextureResource

Synchronously loads a texture resource from a URL.

static func loadAsync(named: String, in: Bundle?) -> LoadRequest&lt;TextureResource>

Returns a load request that creates a texture resource by asynchronously loading it from a bundle.

Deprecated

static func loadAsync(named: String, in: Bundle?, options: TextureResource.CreateOptions) -> LoadRequest&lt;TextureResource>

Returns a load request that creates a texture resource by asynchronously loading it from a bundle with options.

Deprecated

static func loadAsync(contentsOf: URL, withName: String?) -> LoadRequest&lt;TextureResource>

Asynchronously loads a texture resource from a URL.

Deprecated

