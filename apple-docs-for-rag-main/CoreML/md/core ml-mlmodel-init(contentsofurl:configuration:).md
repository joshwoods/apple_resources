

- Core ML
- MLModel
-  init(contentsOfURL:configuration:) 

Initializer

# init(contentsOfURL:configuration:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
convenience init(
    contentsOfURL url: URL,
    configuration: MLModelConfiguration
) throws
```

## See Also

### Loading a Model

class func load(contentsOf: URL, configuration: MLModelConfiguration) async throws -> MLModel

Construct a model asynchronously from a compiled model asset.

class func load(MLModelAsset, configuration: MLModelConfiguration, completionHandler: (MLModel?, (any Error)?) -> Void)

Construct a model asynchronously from a compiled model asset.

class func load(contentsOf: URL, configuration: MLModelConfiguration, completionHandler: (Result&lt;MLModel, any Error>) -> Void)

Creates a Core ML model instance asynchronously from a compiled model file, a custom configuration, and a completion handler.

convenience init(contentsOf: URL) throws

Creates a Core ML model instance from a compiled model file.

convenience init(contentsOf: URL, configuration: MLModelConfiguration) throws

Creates a Core ML model instance from a compiled model file and a custom configuration.

convenience init(contentsOfURL: URL) throws

