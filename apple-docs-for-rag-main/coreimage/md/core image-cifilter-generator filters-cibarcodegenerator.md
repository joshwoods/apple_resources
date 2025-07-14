

- Core Image
- CIFilter
- Generator Filters
-  CIBarcodeGenerator 

Protocol

# CIBarcodeGenerator

The properties you use to configure a barcode generator filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIBarcodeGenerator
```

## Topics

### Instance Properties

var barcodeDescriptor: CIBarcodeDescriptor

The barcode descriptor to generate an image for.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func barcodeGenerator() -> any CIFilter &amp; CIBarcodeGenerator

Generates a barcode as an image from the descriptor.

