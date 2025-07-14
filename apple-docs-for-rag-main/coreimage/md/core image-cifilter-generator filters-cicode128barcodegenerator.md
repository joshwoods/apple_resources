

- Core Image
- CIFilter
- Generator Filters
-  CICode128BarcodeGenerator 

Protocol

# CICode128BarcodeGenerator

The properties you use to configure a Code 128 barcode generator filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CICode128BarcodeGenerator
```

## Topics

### Instance Properties

var barcodeHeight: Float

The height, in pixels, of the generated barcode.

**Required**

var message: Data

The message to encode in the Code 128 barcode.

**Required**

var quietSpace: Float

The number of empty white pixels that should surround the barcode.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func code128BarcodeGenerator() -> any CIFilter &amp; CICode128BarcodeGenerator

Generates a high-density, linear barcode.

