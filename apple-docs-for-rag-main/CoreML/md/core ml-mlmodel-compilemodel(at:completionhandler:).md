

- Core ML
- MLModel
-  compileModel(at:completionHandler:) 

Type Method

# compileModel(at:completionHandler:)

Compile a model for a device.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class func compileModel(
    at url: URL,
    completionHandler handler: @escaping (Result) -> Void
)
```

## Parameters 

`url`  

The URL to the model file.

`handler`  

The completion handler the framework calls when the compilation completes.

## See Also

### Compiling a Model

class func compileModel(at: URL) async throws -> URL

Compile a model for a device.

class func compileModel(at: URL) async throws -> URL

Compile a model for a device.

class func compileModel(at: URL) throws -> URL

Compiles a model on the device to update the model in your app.

Deprecated

