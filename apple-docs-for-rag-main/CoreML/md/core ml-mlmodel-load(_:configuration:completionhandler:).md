

- Core ML
- MLModel
-  load(\_:configuration:completionHandler:) 

Type Method

# load(\_:configuration:completionHandler:)

Construct a model asynchronously from a compiled model asset.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
class func load(
    _ asset: MLModelAsset,
    configuration: MLModelConfiguration,
    completionHandler handler: @escaping (MLModel?, (any Error)?) -> Void
)
```

``` source
class func load(
    asset: MLModelAsset,
    configuration: MLModelConfiguration
) async throws -> MLModel
```

## Parameters 

`asset`  

The compiled model asset derived from in-memory or on-disk Core ML model.

`configuration`  

The model configuration that holds options for loading the model.

`handler`  

The completion handler invoked when the load completes. A valid MLModel returns on success, or an error if failure.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func load(asset: MLModelAsset, configuration: MLModelConfiguration) async throws -> MLModel
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Loading a Model

class func load(contentsOf: URL, configuration: MLModelConfiguration) async throws -> MLModel

Construct a model asynchronously from a compiled model asset.

class func load(contentsOf: URL, configuration: MLModelConfiguration, completionHandler: (Result&lt;MLModel, any Error>) -> Void)

Creates a Core ML model instance asynchronously from a compiled model file, a custom configuration, and a completion handler.

convenience init(contentsOf: URL) throws

Creates a Core ML model instance from a compiled model file.

convenience init(contentsOf: URL, configuration: MLModelConfiguration) throws

Creates a Core ML model instance from a compiled model file and a custom configuration.

convenience init(contentsOfURL: URL) throws

convenience init(contentsOfURL: URL, configuration: MLModelConfiguration) throws

