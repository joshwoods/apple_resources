

- Core ML
- MLModelError
- MLModelError.Code
-  MLModelError.Code.modelDecryptionKeyFetch 

Case

# MLModelError.Code.modelDecryptionKeyFetch

An error code for problems related to retrieving a model’s decryption key.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
case modelDecryptionKeyFetch
```

## Discussion

Core ML typically throws (Swift) or returns (Objective-C) this error when the device doesn’t have access to the network.

## See Also

### Error Codes

case featureType

An error code for problems related to model features.

case parameters

An error code for problems related to model parameters.

case modelCollection

An error code for problems related to retrieving a model collection from the deployment system.

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

