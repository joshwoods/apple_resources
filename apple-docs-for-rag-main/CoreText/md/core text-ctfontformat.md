

- Core Text
-  CTFontFormat 

Enumeration

# CTFontFormat

The recognized format of the font.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CTFontFormat
```

## Overview

Use the values of this enumeration for kCTFontFormatAttribute.

## Topics

### Font Formats

case unrecognized

The font is not a recognized format.

case openTypePostScript

The font is an OpenType format containing PostScript data.

case openTypeTrueType

The font is an OpenType format containing TrueType data.

case trueType

The font is a recognized TrueType format.

case postScript

The font is a recognized PostScript format.

case bitmap

The font is a bitmap-only format.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Related Documentation

let kCTFontFormatAttribute: CFString

The recognized format of the font.

### Accessing Font Attributes

Font Attributes

The keys for accessing font attributes from a font descriptor.

enum CTFontOrientation

The intended rendering orientation of the font for obtaining glyph metrics.

typealias CTFontPriority

The priority of font descriptors when resolving duplicates and sorting match results.

