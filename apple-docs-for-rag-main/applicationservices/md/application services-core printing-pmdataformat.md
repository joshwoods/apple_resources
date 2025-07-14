

- Application Services
- Core Printing
-  PMDataFormat 

Structure

# PMDataFormat

Constants that specify the format of the data representation created with the functions PMPageFormatCreateDataRepresentation(_:_:_:) and PMPrintSettingsCreateDataRepresentation(_:_:_:).

macOS 10.5+

``` source
struct PMDataFormat
```

## Topics

### Constants

var kPMDataFormatXMLDefault: PMDataFormat

var kPMDataFormatXMLMinimal: PMDataFormat

var kPMDataFormatXMLCompressed: PMDataFormat

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

## Relationships

### Conforms To

- Hashable
- RawRepresentable

