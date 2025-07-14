

- RealityKit
- Entity
-  loadAsync(named:in:) Deprecated

Type Method

# loadAsync(named:in:)

Returns a load request that creates an entity by asynchronously loading it from a bundle.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 10.15–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor @preconcurrency
static func loadAsync(
    named name: String,
    in bundle: Bundle? = nil
) -> LoadRequest
```

## Parameters 

`name`  

The base name of the file to load, omitting the filename extension.

`bundle`  

The bundle containing the file. Use `nil` to search the app’s main bundle.

## Return Value

A resource loader that publishes the root entity in the loaded file.

## Mentioned in 

Loading remote assets in multiplayer apps

## Discussion

RealityKit supports loading entities from USD (`.usd`, `.usda`, `.usdc`, `.usdz`) and Reality (`.reality`) files.

When building your app, Xcode automatically converts any Reality Composer projects (`.rcproject`) in the selected target into Reality files, which it then copies into your app’s bundle.

For more information on loading entities, see Loading entities from a file.

## See Also

### Loading an entity hierarchy

static func load(named: String, in: Bundle?) throws -> Entity

Returns an entity by synchronously loading it from a bundle.

static func load(contentsOf: URL, withName: String?) throws -> Entity

Returns an entity by synchronously loading it from a file URL.

static func loadAsync(contentsOf: URL, withName: String?) -> LoadRequest&lt;Entity>

Returns a load request that creates an entity by asynchronously loading it from a file URL and preserving the entity’s hierarchy.

Deprecated

