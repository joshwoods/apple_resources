

- RealityKit
- Entity
-  load(contentsOf:withName:) 

Type Method

# load(contentsOf:withName:)

Returns an entity by synchronously loading it from a file URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
static func load(
    contentsOf url: URL,
    withName resourceName: String? = nil
) throws -> Entity
```

## Parameters 

`url`  

A file URL representing the file to load.

`resourceName`  

A unique name the method assigns to the resource it loads, for use in network synchronization.

## Return Value

The root entity in the loaded file.

## Mentioned in 

Loading entities from a file

Taking Control of Scene Anchoring

## Discussion

Loading an Entity with this method blocks the main actor because it’s synchronous, so only call it from a command-line application. The method can stall a regular app, which makes it visibly hitch, and the system terminates an app if its UI becomes unresponsive. See init(named:in:) for an example that demonstrates how to safely load content.

RealityKit supports loading entities from USD (`.usd`, `.usda`, `.usdc`, `.usdz`) and Reality (`.reality`) files.

When building your app, Xcode automatically converts any Reality Composer projects (`.rcproject`) in the selected target into Reality files, which it then copies into your app’s bundle.

For more information on loading entities, see Loading entities from a file.

## See Also

### Loading an entity hierarchy

static func load(named: String, in: Bundle?) throws -> Entity

Returns an entity by synchronously loading it from a bundle.

static func loadAsync(named: String, in: Bundle?) -> LoadRequest&lt;Entity>

Returns a load request that creates an entity by asynchronously loading it from a bundle.

Deprecated

static func loadAsync(contentsOf: URL, withName: String?) -> LoadRequest&lt;Entity>

Returns a load request that creates an entity by asynchronously loading it from a file URL and preserving the entity’s hierarchy.

Deprecated

