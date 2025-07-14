

- ShazamKit
- SHError
- SHError.Code
-  SHError.Code.signatureDurationInvalid 

Case

# SHError.Code.signatureDurationInvalid

The error code to indicate that the length of the generated signature is too long or too short to make a match in the catalog.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case signatureDurationInvalid
```

## Discussion

This error occurs when the length of the generated signature is less than minimumQuerySignatureDuration or greater than maximumQuerySignatureDuration for the session catalog.

## See Also

### Signature errors

case signatureInvalid

The error code to indicate that the system is unable to generate a signature from the audio.

