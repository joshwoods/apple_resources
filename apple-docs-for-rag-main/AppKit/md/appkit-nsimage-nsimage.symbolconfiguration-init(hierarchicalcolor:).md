

- AppKit
- NSImage
- NSImage.SymbolConfiguration
-  init(hierarchicalColor:) 

Initializer

# init(hierarchicalColor:)

Creates a hierarchical color configuration using the color you specify.

macOS 12.0+

``` source
convenience init(hierarchicalColor: NSColor)
```

## Parameters 

`hierarchicalColor`  

The primary color for the symbol.

## Return Value

A new configuration object that creates a palette from a primary color.

## Discussion

This method creates a color scheme based on a single color. The system reduces the intensity of the base color to create the secondary and tertiary colors.

When combining this with another configuration, the last configuration overrides existing values.

If the symbol doesn’t have a palette variant, this color configuration doesn’t have an effect, so the symbol uses the monochrome (templated) symbol.

## See Also

### Creating a Color Configuration

convenience init(paletteColors: [NSColor])

Creates a color configuration by specifying a palette of colors.

class func preferringMulticolor() -> Self

Creates a configuration that specifies that the symbol should prefer its multicolor variant if one exists.

