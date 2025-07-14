

- AVFoundation
- AVCaptionConversionValidator
-  warnings 

Instance Property

# warnings

The collection of warnings the validator encountered.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var warnings: [AVCaptionConversionWarning] { get }
```

## Discussion

This property value may change while the validator’s status is AVCaptionConversionValidator.Status.validating.

## See Also

### Validating Captions

func validateCaptionConversion(warningHandler: (AVCaptionConversionWarning?) -> Void)

Validates the object’s captions.

class AVCaptionConversionWarning

An object that represents a conversion warning produced by a validator.

func stopValidating()

Stops the active validation operation.

