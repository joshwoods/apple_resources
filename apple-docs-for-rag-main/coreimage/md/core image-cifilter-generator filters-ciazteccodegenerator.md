

- Core Image
- CIFilter
- Generator Filters
-  CIAztecCodeGenerator 

Protocol

# CIAztecCodeGenerator

The properties you use to configure an Aztec code generator filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIAztecCodeGenerator
```

## Topics

### Instance Properties

var compactStyle: Float

A Boolean that specifies whether to force a compact style Aztec code.

**Required**

var correctionLevel: Float

The Aztec error correction, a value from 5 to 95.

**Required**

var layers: Float

The number of Aztec layers, a value from 1 to 32.

**Required**

var message: Data

The message to encode in the Aztec barcode.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func aztecCodeGenerator() -> any CIFilter &amp; CIAztecCodeGenerator

Generates a low-density barcode.

