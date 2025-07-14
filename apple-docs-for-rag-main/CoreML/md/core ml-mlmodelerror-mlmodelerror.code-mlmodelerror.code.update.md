

- Core ML
- MLModelError
- MLModelError.Code
-  MLModelError.Code.update 

Case

# MLModelError.Code.update

An error code for problems related to on-device model updates.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
case update
```

## Discussion

Core ML typically throws (Swift) or returns (Objective-C) this error when the update process encounters a problem at runtime, such as an MLMultiArray input with an incorrect shape.

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

