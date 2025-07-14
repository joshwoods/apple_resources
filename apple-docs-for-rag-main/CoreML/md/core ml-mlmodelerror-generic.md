

- Core ML
- MLModelError
-  generic 

Type Property

# generic

An error code for runtime issues that don’t apply to the other error codes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
static var generic: MLModelError.Code { get }
```

## Discussion

Core ML typically throws this error when it encounters an internal problem.

## See Also

### Error Codes

static var featureType: MLModelError.Code

An error code for problems related to model features.

static var parameters: MLModelError.Code

An error code for problems related to model parameters.

static var modelCollection: MLModelError.Code

An error code for problems related to retrieving a model collection from the deployment system.

static var modelDecryptionKeyFetch: MLModelError.Code

An error code for problems related to retrieving a model’s decryption key.

static var modelDecryption: MLModelError.Code

An error code for problems related to decrypting models.

static var update: MLModelError.Code

An error code for problems related to on-device model updates.

static var customLayer: MLModelError.Code

An error code for problems related to custom layers.

static var customModel: MLModelError.Code

An error code for problems related to custom models.

static var io: MLModelError.Code

An error code for problems related to the system’s input or output.

static var predictionCancelled: MLModelError.Code

An error code for problems related to cancelling the prediction before it completes.

enum Code

Information about a Core ML model error.

