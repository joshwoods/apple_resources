

- Core Image
- CIQRCodeDescriptor
-  errorCorrectionLevel 

Instance Property

# errorCorrectionLevel

The QR code error correction level.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var errorCorrectionLevel: CIQRCodeDescriptor.ErrorCorrectionLevel { get }
```

## Discussion

The possible error correction levels of CIQRCodeDescriptor.ErrorCorrectionLevel are enumerated as follows:

- CIQRCodeDescriptor.ErrorCorrectionLevel.levelL = 'L'

- CIQRCodeDescriptor.ErrorCorrectionLevel.levelM = 'M'

- CIQRCodeDescriptor.ErrorCorrectionLevel.levelQ = 'Q'

- CIQRCodeDescriptor.ErrorCorrectionLevel.levelH = 'H'

## See Also

### Examining a Descriptor

var errorCorrectedPayload: Data

The error-corrected payload containing the data encoded in the QR code.

var symbolVersion: Int

The version of the QR code.

var maskPattern: UInt8

The QR code's mask pattern.

