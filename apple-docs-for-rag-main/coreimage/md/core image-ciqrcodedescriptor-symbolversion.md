

- Core Image
- CIQRCodeDescriptor
-  symbolVersion 

Instance Property

# symbolVersion

The version of the QR code.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var symbolVersion: Int { get }
```

## Discussion

ISO/IEC 18004 defines versions from 1 to 40, where a higher symbol version indicates a larger data-carrying capacity

## See Also

### Examining a Descriptor

var errorCorrectedPayload: Data

The error-corrected payload containing the data encoded in the QR code.

var maskPattern: UInt8

The QR code's mask pattern.

var errorCorrectionLevel: CIQRCodeDescriptor.ErrorCorrectionLevel

The QR code error correction level.

