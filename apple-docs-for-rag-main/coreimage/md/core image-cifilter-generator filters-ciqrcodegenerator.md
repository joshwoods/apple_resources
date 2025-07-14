

- Core Image
- CIFilter
- Generator Filters
-  CIQRCodeGenerator 

Protocol

# CIQRCodeGenerator

The properties you use to configure a QR code generator filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIQRCodeGenerator
```

## Topics

### Instance Properties

var correctionLevel: String

The QR code correction level: L, M, Q, or H.

**Required**

var message: Data

The message to encode in the QR code.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func qrCodeGenerator() -> any CIFilter &amp; CIQRCodeGenerator

Generates a quick response (QR) code image.

