

- Core ML
- MLModel
-  load(contentsOf:configuration:) 

Type Method

# load(contentsOf:configuration:)

Construct a model asynchronously from a compiled model asset.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class func load(
    contentsOf url: URL,
    configuration: MLModelConfiguration = MLModelConfiguration()
) async throws -> MLModel
```

## Parameters 

`url`  

The URL of the compiled model asset derived from in-memory or on-disk Core ML model.

`configuration`  

The model configuration that hold options for loading the model.

## Return Value

The loaded model, if successful; otherwise, `nil`.

## See Also

### Loading a Model

class func load(MLModelAsset, configuration: MLModelConfiguration, completionHandler: (MLModel?, (any Error)?) -> Void)

Construct a model asynchronously from a compiled model asset.

class func load(contentsOf: URL, configuration: MLModelConfiguration, completionHandler: (Result&lt;MLModel, any Error>) -> Void)

Creates a Core ML model instance asynchronously from a compiled model file, a custom configuration, and a completion handler.

convenience init(contentsOf: URL) throws

Creates a Core ML model instance from a compiled model file.

convenience init(contentsOf: URL, configuration: MLModelConfiguration) throws

Creates a Core ML model instance from a compiled model file and a custom configuration.

convenience init(contentsOfURL: URL) throws

convenience init(contentsOfURL: URL, configuration: MLModelConfiguration) throws

