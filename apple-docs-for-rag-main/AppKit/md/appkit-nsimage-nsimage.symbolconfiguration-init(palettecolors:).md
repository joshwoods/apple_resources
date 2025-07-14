

- AppKit
- NSImage
- NSImage.SymbolConfiguration
-  init(paletteColors:) 

Initializer

# init(paletteColors:)

Creates a color configuration by specifying a palette of colors.

macOS 12.0+

``` source
convenience init(paletteColors: [NSColor])
```

## Parameters 

`paletteColors`  

The colors to apply to the symbol.

## Return Value

A new configuration object that prefers its palette variant.

## Discussion

The system applies the colors sequentially per layer — the first color for the first layer, and the second color for the second layer. This is independent of the hierarchy level of the layer.

When you combine this with another configuration to create a palette, the last configuration overrides any existing color configuration.

If the symbol doesn’t have a palette variant, this color configuration doesn’t have an effect, so the symbol uses the monochrome (templated) symbol.

## See Also

### Creating a Color Configuration

convenience init(hierarchicalColor: NSColor)

Creates a hierarchical color configuration using the color you specify.

class func preferringMulticolor() -> Self

Creates a configuration that specifies that the symbol should prefer its multicolor variant if one exists.

