

- RealityKit
- Entity
-  loadAsync(contentsOf:withName:) Deprecated

Type Method

# loadAsync(contentsOf:withName:)

Returns a load request that creates an entity by asynchronously loading it from a file URL and preserving the entity’s hierarchy.

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

The location of a file that represents an entity.

`resourceName`  

A unique name the method assigns to the resource it loads, for use in network synchronization.

## Mentioned in 

Taking Control of Scene Anchoring

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

static func loadAsync(named: String, in: Bundle?) -> LoadRequest&lt;Entity>

Returns a load request that creates an entity by asynchronously loading it from a bundle.

Deprecated

