

- Core Image
- CIQRCodeFeature
-  symbolDescriptor 

Instance Property

# symbolDescriptor

An abstract representation of a QR Code symbol.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var symbolDescriptor: CIQRCodeDescriptor? { get }
```

## Discussion

Concrete subclass of CIBarcodeDescriptor. Contains the payload, version of the symbol, mask pattern, and error correction level, so the QR Code can be reproduced.

## See Also

### Decoding a Detected Barcode

var messageString: String?

The string decoded from the detected barcode.

