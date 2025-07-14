

- RealityKit
- Entity
-  loadModel(contentsOf:withName:) 

Type Method

# loadModel(contentsOf:withName:)

Synchronously loads a model entity from a file URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
static func loadModel(
    contentsOf url: URL,
    withName resourceName: String? = nil
) throws -> ModelEntity
```

## Parameters 

`url`  

A file URL representing the file to load.

`resourceName`  

A unique name the method assigns to the resource it loads, for use in network synchronization.

## Return Value

The root entity in the loaded file, which Reality Kit casts as a ModelEntity.

## Mentioned in 

Loading Reality Composer files manually without generated code

## Discussion

Loading an Entity with this method blocks the main actor because it’s synchronous, so only call it from a command-line application. The method can stall a regular app, which makes it visibly hitch, and the system terminates an app if its UI becomes unresponsive. See init(named:in:) for an example that demonstrates how to safely load content.

## See Also

### Loading a flattened model entity

static func loadModel(named: String, in: Bundle?) throws -> ModelEntity

Synchronously loads a model entity from a bundle.

static func loadModelAsync(named: String, in: Bundle?) -> LoadRequest&lt;ModelEntity>

Asynchronously loads a model entity from a bundle.

Deprecated

static func loadModelAsync(contentsOf: URL, withName: String?) -> LoadRequest&lt;ModelEntity>

Returns a load request that creates a model entity by asynchronously loading it from a file URL and flattening the model entity’s hierarchy.

Deprecated

