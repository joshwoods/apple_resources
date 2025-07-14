

- AppKit
- NSImage
-  NSImage.SymbolScale 

Enumeration

# NSImage.SymbolScale

Constants that specify which scale variant of a symbol image to use.

macOS 11.0+

``` source
enum SymbolScale
```

## Overview

Specify a different scale variant for a symbol to change the emphasis of the symbol relative to its adjacent text. The default symbol scale is NSImage.SymbolScale.medium.

## Topics

### Constants

case small

The symbol uses the small scale variant.

case medium

The symbol uses the default medium scale variant.

case large

The symbol uses the large scale variant.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating a Symbol Configuration

convenience init(pointSize: CGFloat, weight: NSFont.Weight)

Creates a symbol configuration with the specified point size and font weight.

convenience init(pointSize: CGFloat, weight: NSFont.Weight, scale: NSImage.SymbolScale)

Creates a symbol configuration with the specified point size, font weight, and symbol scale.

convenience init(textStyle: NSFont.TextStyle)

Creates a symbol configuration with the specified text style.

convenience init(textStyle: NSFont.TextStyle, scale: NSImage.SymbolScale)

Creates a symbol configuration with the specified text style and symbol scale.

convenience init(scale: NSImage.SymbolScale)

Creates a symbol configuration using the scale you specify.

struct TextStyle

Constants that specify the preferred text styles you use with fonts.

