

- Core ML
- MLModelError
- MLModelError.Code
-  MLModelError.Code.parameters 

Case

# MLModelError.Code.parameters

An error code for problems related to model parameters.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case parameters
```

## Discussion

Core ML typically throws (Swift) or returns (Objective-C) this error when an app queries the model for a parameter it doesn’t support.

## See Also

### Error Codes

case featureType

An error code for problems related to model features.

case modelCollection

An error code for problems related to retrieving a model collection from the deployment system.

case modelDecryptionKeyFetch

An error code for problems related to retrieving a model’s decryption key.

case modelDecryption

An error code for problems related to decrypting models.

case update

An error code for problems related to on-device model updates.

case customLayer

An error code for problems related to custom layers.

case customModel

An error code for problems related to custom models.

case io

An error code for problems related to the system’s input or output.

case predictionCancelled

An error code for problems related to canceling the prediction before it completes.

case generic

An error code for runtime issues that don’t apply to the other error codes.

