

- AppKit
- NSImage
- NSImage.SymbolConfiguration
-  init(textStyle:scale:) 

Initializer

# init(textStyle:scale:)

Creates a symbol configuration with the specified text style and symbol scale.

macOS 11.0+

``` source
convenience init(
    textStyle style: NSFont.TextStyle,
    scale: NSImage.SymbolScale
)
```

## See Also

### Creating a Symbol Configuration

convenience init(pointSize: CGFloat, weight: NSFont.Weight)

Creates a symbol configuration with the specified point size and font weight.

convenience init(pointSize: CGFloat, weight: NSFont.Weight, scale: NSImage.SymbolScale)

Creates a symbol configuration with the specified point size, font weight, and symbol scale.

convenience init(textStyle: NSFont.TextStyle)

Creates a symbol configuration with the specified text style.

convenience init(scale: NSImage.SymbolScale)

Creates a symbol configuration using the scale you specify.

struct TextStyle

Constants that specify the preferred text styles you use with fonts.

enum SymbolScale

Constants that specify which scale variant of a symbol image to use.

