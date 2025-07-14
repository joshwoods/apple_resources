

- Core ML
- MLModelError
- MLModelError.Code
-  MLModelError.Code.customModel 

Case

# MLModelError.Code.customModel

An error code for problems related to custom models.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
case customModel
```

## Discussion

Core ML typically throws (Swift) or returns (Objective-C) this error when the custom model has a programming mistake. For example, a custom model’s prediction method fails with this error code if Core ML can’t find the custom model’s implementation.

## See Also

### Error Codes

case featureType

An error code for problems related to model features.

case parameters

An error code for problems related to model parameters.

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

case io

An error code for problems related to the system’s input or output.

case predictionCancelled

An error code for problems related to canceling the prediction before it completes.

case generic

An error code for runtime issues that don’t apply to the other error codes.

