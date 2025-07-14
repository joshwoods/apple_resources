

- RealityKit
- Entity
-  loadModelAsync(contentsOf:withName:) Deprecated

Type Method

# loadModelAsync(contentsOf:withName:)

Returns a load request that creates a model entity by asynchronously loading it from a file URL and flattening the model entity’s hierarchy.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 10.15–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor @preconcurrency
static func loadModelAsync(
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

Loading Reality Composer files manually without generated code

## Discussion

For more information on loading entities, see Loading entities from a file.

## See Also

### Loading a flattened model entity

static func loadModel(named: String, in: Bundle?) throws -> ModelEntity

Synchronously loads a model entity from a bundle.

static func loadModel(contentsOf: URL, withName: String?) throws -> ModelEntity

Synchronously loads a model entity from a file URL.

static func loadModelAsync(named: String, in: Bundle?) -> LoadRequest&lt;ModelEntity>

Asynchronously loads a model entity from a bundle.

Deprecated

