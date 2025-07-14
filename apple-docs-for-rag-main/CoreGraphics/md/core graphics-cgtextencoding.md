

- Core Graphics
-  CGTextEncoding 

Enumeration

# CGTextEncoding

Text encodings for fonts.

tvOSvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
enum CGTextEncoding
```

## Overview

For more information on setting the font in a graphics context, see selectFont(name:size:textEncoding:).

## Topics

### Constants

case encodingFontSpecific

The built-in encoding of the font.

case encodingMacRoman

The MacRoman encoding. MacRoman is an ASCII variant originally created for use in the Mac OS, in which characters 127 and lower are ASCII, and characters 128 and higher are non-English characters and symbols.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum CGPathFillRule

Rules for determining which regions are interior to a path, used by the fillPath(using:) and clip(using:) methods.

