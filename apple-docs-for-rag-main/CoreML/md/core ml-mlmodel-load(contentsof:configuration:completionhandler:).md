

- Core ML
- MLModel
-  load(contentsOf:configuration:completionHandler:) 

Type Method

# load(contentsOf:configuration:completionHandler:)

Creates a Core ML model instance asynchronously from a compiled model file, a custom configuration, and a completion handler.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class func load(
    contentsOf url: URL,
    configuration: MLModelConfiguration = MLModelConfiguration(),
    completionHandler handler: @escaping (Result) -> Void
)
```

## Parameters 

`url`  

The path to a compiled model file (*ModelName*`.mlmodelc`), typically with the `URL` that compileModel(at:) returns.

`configuration`  

The runtime settings for the new model instance.

`handler`  

A closure the method calls when it finishes loading the model.

## Discussion

Use this method to load a model asynchronously. Core ML calls your completion handler after it successfully loads the model, or encounters an error attempting to load it.

- Swift
- Objective-C

```
MLModel.load(contentsOf: modelURL) { result in
    switch result {
    case .success(let loadedModel):
        print("Successfully loaded model `\(loadedModel)`.")

        // Use the loaded model for predictions.
        // ...

    case .failure(let error):
        print("Error loading model: \(error).")
    }
}
```

```
```

In Swift, if the model loaded successfully, you can use the instance from the Result.success(_:) associated value; otherwise, use the Result.failure(_:) associated value to address the error. In Objective-C, you can use the MLModel instance in your completion hander; otherwise, use the NSError instance to address the error. See MLModelError.Code for the list of error codes.

## See Also

### Loading a Model

class func load(contentsOf: URL, configuration: MLModelConfiguration) async throws -> MLModel

Construct a model asynchronously from a compiled model asset.

class func load(MLModelAsset, configuration: MLModelConfiguration, completionHandler: (MLModel?, (any Error)?) -> Void)

Construct a model asynchronously from a compiled model asset.

convenience init(contentsOf: URL) throws

Creates a Core ML model instance from a compiled model file.

convenience init(contentsOf: URL, configuration: MLModelConfiguration) throws

Creates a Core ML model instance from a compiled model file and a custom configuration.

convenience init(contentsOfURL: URL) throws

convenience init(contentsOfURL: URL, configuration: MLModelConfiguration) throws

