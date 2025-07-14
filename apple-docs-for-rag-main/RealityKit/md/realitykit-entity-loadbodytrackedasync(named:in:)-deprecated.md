

- RealityKit
- Entity
-  loadBodyTrackedAsync(named:in:) Deprecated

Type Method

# loadBodyTrackedAsync(named:in:)

Asynchronously loads a body-tracked entity from a bundle.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.0–18.0Deprecated

``` source
@MainActor @preconcurrency
static func loadBodyTrackedAsync(
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

A resource loader that publishes the root entity in the loaded file as a BodyTrackedEntity.

## See Also

### Loading a flattened body-tracked entity

static func loadBodyTracked(named: String, in: Bundle?) throws -> BodyTrackedEntity

Synchronously loads a body-tracked entity from a bundle.

static func loadBodyTracked(contentsOf: URL, withName: String?) throws -> BodyTrackedEntity

Synchronously loads a body-tracked entity from a file URL.

static func loadBodyTrackedAsync(contentsOf: URL, withName: String?) -> LoadRequest&lt;BodyTrackedEntity>

Asynchronously loads a body-tracked entity from a file URL.

