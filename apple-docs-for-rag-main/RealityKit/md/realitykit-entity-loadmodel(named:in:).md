

- RealityKit
- Entity
-  loadModel(named:in:) 

Type Method

# loadModel(named:in:)

Synchronously loads a model entity from a bundle.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
static func loadModel(
    named name: String,
    in bundle: Bundle? = nil
) throws -> ModelEntity
```

## Parameters 

`name`  

The base name of the file to load, omitting the filename extension.

`bundle`  

The bundle containing the file. Use `nil` to search the app’s main bundle.

## Return Value

The root entity in the loaded file, which Reality Kit casts as a ModelEntity.

## Mentioned in 

Reducing CPU Utilization in Your RealityKit App

Loading entities from a file

## Discussion

Loading an Entity with this method blocks the main actor because it’s synchronous, so only call it from a command-line application. The method can stall a regular app, which makes it visibly hitch, and the system terminates an app if its UI becomes unresponsive. See init(named:in:) for an example that demonstrates how to safely load content.

## See Also

### Loading a flattened model entity

static func loadModel(contentsOf: URL, withName: String?) throws -> ModelEntity

Synchronously loads a model entity from a file URL.

static func loadModelAsync(named: String, in: Bundle?) -> LoadRequest&lt;ModelEntity>

Asynchronously loads a model entity from a bundle.

Deprecated

static func loadModelAsync(contentsOf: URL, withName: String?) -> LoadRequest&lt;ModelEntity>

Returns a load request that creates a model entity by asynchronously loading it from a file URL and flattening the model entity’s hierarchy.

Deprecated

