

- AVFoundation
- AVCaptionConversionValidator
-  stopValidating() 

Instance Method

# stopValidating()

Stops the active validation operation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
func stopValidating()
```

## Discussion

You can call this method at any time, even within the validator’s callback to its handler.

Calling this method stops validation and changes the status value to AVCaptionConversionValidator.Status.stopped.

## See Also

### Validating Captions

func validateCaptionConversion(warningHandler: (AVCaptionConversionWarning?) -> Void)

Validates the object’s captions.

var warnings: [AVCaptionConversionWarning]

The collection of warnings the validator encountered.

class AVCaptionConversionWarning

An object that represents a conversion warning produced by a validator.

