

- RealityKit
- Entity
-  loadAnchorAsync(named:in:) Deprecated

Type Method

# loadAnchorAsync(named:in:)

Asynchronously loads an anchor entity from a bundle.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 10.15–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor @preconcurrency
static func loadAnchorAsync(
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

A resource loader that publishes the root entity in the loaded file as an AnchorEntity.

## See Also

### Loading an anchor entity

static func loadAnchor(named: String, in: Bundle?) throws -> AnchorEntity

Synchronously loads an anchor entity from a bundle.

static func loadAnchor(contentsOf: URL, withName: String?) throws -> AnchorEntity

Synchronously loads an anchor entity from a file URL.

static func loadAnchorAsync(contentsOf: URL, withName: String?) -> LoadRequest&lt;AnchorEntity>

Asynchronously loads an anchor entity from a file URL.

Deprecated

