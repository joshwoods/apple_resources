

- AVFoundation
- AVCaptionConversionValidator
-  validateCaptionConversion(warningHandler:) 

Instance Method

# validateCaptionConversion(warningHandler:)

Validates the object’s captions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
func validateCaptionConversion(warningHandler handler: @escaping (AVCaptionConversionWarning?) -> Void)
```

## Parameters 

`handler`  

The callback the system invokes when it finishes validation.

## Discussion

When the object finishes validating and reports all warnings, it invokes the callback once with a value of `nil` for its warning parameter. When this occurs, the validator’s status value changes to AVCaptionConversionValidator.Status.completed.

Stop an in-progress validation operation by calling stopValidating().

Important

It’s only valid to call this method when the validator’s state is AVCaptionConversionValidator.Status.unknown.

## See Also

### Validating Captions

var warnings: [AVCaptionConversionWarning]

The collection of warnings the validator encountered.

class AVCaptionConversionWarning

An object that represents a conversion warning produced by a validator.

func stopValidating()

Stops the active validation operation.

