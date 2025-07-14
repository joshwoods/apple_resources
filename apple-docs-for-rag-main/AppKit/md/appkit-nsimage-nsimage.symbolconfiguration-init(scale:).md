

- AppKit
- NSImage
- NSImage.SymbolConfiguration
-  init(scale:) 

Initializer

# init(scale:)

Creates a symbol configuration using the scale you specify.

macOS 11.0+

``` source
convenience init(scale: NSImage.SymbolScale)
```

## Parameters 

`scale`  

The symbol scale.

## Return Value

A new configuration object.

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

struct TextStyle

Constants that specify the preferred text styles you use with fonts.

enum SymbolScale

Constants that specify which scale variant of a symbol image to use.

