

- RealityKit
- Entity
-  loadAnchorAsync(contentsOf:withName:) Deprecated

Type Method

# loadAnchorAsync(contentsOf:withName:)

Asynchronously loads an anchor entity from a file URL.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 10.15–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor @preconcurrency
static func loadAnchorAsync(
    contentsOf url: URL,
    withName resourceName: String? = nil
) -> LoadRequest
```

## Parameters 

`url`  

A file URL representing the file to load.

`resourceName`  

A unique name the method assigns to the resource it loads, for use in network synchronization.

## Return Value

A resource loader that publishes the root entity in the loaded file as an AnchorEntity.

## Mentioned in 

Loading Reality Composer files manually without generated code

Taking Control of Scene Anchoring

## See Also

### Loading an anchor entity

static func loadAnchor(named: String, in: Bundle?) throws -> AnchorEntity

Synchronously loads an anchor entity from a bundle.

static func loadAnchor(contentsOf: URL, withName: String?) throws -> AnchorEntity

Synchronously loads an anchor entity from a file URL.

static func loadAnchorAsync(named: String, in: Bundle?) -> LoadRequest&lt;AnchorEntity>

Asynchronously loads an anchor entity from a bundle.

Deprecated

