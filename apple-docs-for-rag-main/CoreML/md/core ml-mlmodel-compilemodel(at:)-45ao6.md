

- Core ML
- MLModel
-  compileModel(at:) 

Type Method

# compileModel(at:)

Compile a model for a device.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class func compileModel(at url: URL) async throws -> URL
```

## Parameters 

`url`  

The URL to the model file.

## Return Value

A URL to the compiled model directory, if successful; otherwise, `nil`.

## See Also

### Compiling a Model

class func compileModel(at: URL, completionHandler: (Result&lt;URL, any Error>) -> Void)

Compile a model for a device.

class func compileModel(at: URL) async throws -> URL

Compile a model for a device.

class func compileModel(at: URL) throws -> URL

Compiles a model on the device to update the model in your app.

Deprecated

