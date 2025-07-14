

- Core Image
- CIFilter
- Generator Filters
-  CIPDF417BarcodeGenerator 

Protocol

# CIPDF417BarcodeGenerator

The properties you use to configure a PDF417 barcode generator filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIPDF417BarcodeGenerator
```

## Topics

### Instance Properties

var alwaysSpecifyCompaction: Float

A Boolean value specifying whether to force compaction style.

**Required**

var compactStyle: Float

A Boolean value specifying whether to force compact style Aztec code.

**Required**

var compactionMode: Float

The compaction mode of the generated barcode.

**Required**

var correctionLevel: Float

The correction level ratio of the generated barcode.

**Required**

var dataColumns: Float

The number of data columns in the generated barcode.

**Required**

var maxHeight: Float

The maximum height, in pixels, of the generated barcode.

**Required**

var maxWidth: Float

The maximum width, in pixels, of the generated barcode.

**Required**

var message: Data

The message to encode in the PDF417 barcode.

**Required**

var minHeight: Float

The minimum height, in pixels, of the generated barcode.

**Required**

var minWidth: Float

The minimum width, in pixels, of the generated barcode.

**Required**

var preferredAspectRatio: Float

The preferred aspect ratio of the generated barcode.

**Required**

var rows: Float

The number of rows in the generated barcode.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func pdf417BarcodeGenerator() -> any CIFilter &amp; CIPDF417BarcodeGenerator

Generates a high-density linear barcode.

