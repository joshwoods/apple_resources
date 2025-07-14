

- Core ML
- MLModel
-  init(contentsOf:configuration:) 

Initializer

# init(contentsOf:configuration:)

Creates a Core ML model instance from a compiled model file and a custom configuration.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
convenience init(
    contentsOf url: URL,
    configuration: MLModelConfiguration
) throws
```

## Parameters 

`url`  

The path to a compiled model file (*ModelName*`.mlmodelc`), typically with the `URL` that compileModel(at:) returns.

`configuration`  

The runtime settings for the new model instance.

## Discussion

In most cases, your app won’t need to create a model object directly. Consider the programmer-friendly wrapper class that Xcode automatically generates when you add a model to your project (see Integrating a Core ML Model into Your App).

If the wrapper class doesn’t meet your app’s needs or you need to customize the model’s configuration, use this initializer to create a model object from any compiled model file you can access. Typically, you use this initializer after your app has downloaded and compiled a model, which is one technique for saving space in your app (see Downloading and Compiling a Model on the User’s Device).

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

convenience init(contentsOfURL: URL) throws

convenience init(contentsOfURL: URL, configuration: MLModelConfiguration) throws

