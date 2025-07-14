

- Core ML
- MLModelError
- MLModelError.Code
-  MLModelError.Code.featureType 

Case

# MLModelError.Code.featureType

An error code for problems related to model features.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
case featureType
```

## Discussion

Core ML typically throws (Swift) or returns (Objective-C) this error when an app sends an input feature a value that’s of an incorrect type.

## See Also

### Error Codes

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

case customModel

An error code for problems related to custom models.

case io

An error code for problems related to the system’s input or output.

case predictionCancelled

An error code for problems related to canceling the prediction before it completes.

case generic

An error code for runtime issues that don’t apply to the other error codes.

