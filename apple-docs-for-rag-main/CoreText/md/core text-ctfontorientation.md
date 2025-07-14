

- Core Text
-  CTFontOrientation 

Enumeration

# CTFontOrientation

The intended rendering orientation of the font for obtaining glyph metrics.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CTFontOrientation
```

## Overview

Use the values of this enumeration for kCTFontOrientationAttribute.

## Topics

### Font Orientations

case `default`

The native orientation of the font.

case horizontal

The horizontal orientation.

case vertical

The vertical orientation.

### Deprecated Constants

static var kCTFontDefaultOrientation: CTFontOrientation

The native orientation of the font.

Deprecated

static var kCTFontHorizontalOrientation: CTFontOrientation

The horizontal orientation.

Deprecated

static var kCTFontVerticalOrientation: CTFontOrientation

The vertical orientation.

Deprecated

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

let kCTFontOrientationAttribute: CFString

The orientation for the glyphs of the font.

### Accessing Font Attributes

Font Attributes

The keys for accessing font attributes from a font descriptor.

enum CTFontFormat

The recognized format of the font.

typealias CTFontPriority

The priority of font descriptors when resolving duplicates and sorting match results.

