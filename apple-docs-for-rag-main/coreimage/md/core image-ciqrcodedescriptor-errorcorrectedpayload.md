

- Core Image
- CIQRCodeDescriptor
-  errorCorrectedPayload 

Instance Property

# errorCorrectedPayload

The error-corrected payload containing the data encoded in the QR code.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var errorCorrectedPayload: Data { get }
```

## See Also

### Examining a Descriptor

var symbolVersion: Int

The version of the QR code.

var maskPattern: UInt8

The QR code's mask pattern.

var errorCorrectionLevel: CIQRCodeDescriptor.ErrorCorrectionLevel

The QR code error correction level.

