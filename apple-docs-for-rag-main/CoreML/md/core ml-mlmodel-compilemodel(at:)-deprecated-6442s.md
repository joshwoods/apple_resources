

- Core ML
- MLModel
-  compileModel(at:) Deprecated

Type Method

# compileModel(at:)

Compiles a model on the device to update the model in your app.

iOS 11.0–14.0DeprecatediPadOS 11.0–14.0DeprecatedMac Catalyst 13.1+macOS 10.13–11.0DeprecatedtvOS 11.0+visionOS 1.0–2.4Deprecated

``` source
class func compileModel(at modelURL: URL) throws -> URL
```

Deprecated

Use the asynchronous interface compileModelAtURL:completionHandler:error: instead.

## Parameters 

`modelURL`  

The local file path to your downloaded `.mlmodel` file.

## Return Value

The local file path to the compiled model (the `.mlmodelc` file).

## Mentioned in 

Downloading and Compiling a Model on the User’s Device

## Discussion

The source `.mlmodel` file must be on the device. Pass the compiled model to init(contentsOf:) to initialize an MLModel instance.

Listing 1. Compiling a model file and creating an `MLModel` instance from the compiled version

```
let compiledUrl = try MLModel.compileModel(at: modelUrl)
let model = try MLModel(contentsOf: compiledUrl)
```

Compiling can be time consuming and shouldn’t be done on the main thread.

See Downloading and Compiling a Model on the User’s Device for more details.

## See Also

### Related Documentation

Downloading and Compiling a Model on the User’s Device

Install Core ML models on the user’s device dynamically at runtime.

### Compiling a Model

class func compileModel(at: URL) async throws -> URL

Compile a model for a device.

class func compileModel(at: URL, completionHandler: (Result&lt;URL, any Error>) -> Void)

Compile a model for a device.

class func compileModel(at: URL) async throws -> URL

Compile a model for a device.

