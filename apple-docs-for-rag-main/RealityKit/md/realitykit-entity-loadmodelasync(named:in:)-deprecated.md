

- RealityKit
- Entity
-  loadModelAsync(named:in:) Deprecated

Type Method

# loadModelAsync(named:in:)

Asynchronously loads a model entity from a bundle.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 10.15–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor @preconcurrency
static func loadModelAsync(
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

A resource loader that publishes the root entity in the loaded file as a ModelEntity.

## Mentioned in 

Reducing CPU Utilization in Your RealityKit App

## See Also

### Loading a flattened model entity

static func loadModel(named: String, in: Bundle?) throws -> ModelEntity

Synchronously loads a model entity from a bundle.

static func loadModel(contentsOf: URL, withName: String?) throws -> ModelEntity

Synchronously loads a model entity from a file URL.

static func loadModelAsync(contentsOf: URL, withName: String?) -> LoadRequest&lt;ModelEntity>

Returns a load request that creates a model entity by asynchronously loading it from a file URL and flattening the model entity’s hierarchy.

Deprecated

