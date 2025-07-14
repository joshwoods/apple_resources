

- AppKit
- NSImage
-  symbolConfiguration 

Instance Property

# symbolConfiguration

The configuration details for a symbol image.

macOS 12.0+

``` source
@NSCopying
var symbolConfiguration: NSImage.SymbolConfiguration { get }
```

## Discussion

Use this property to access the traits and rendering attributes the system uses with the symbol image. These details determine which variant of the image to load and draw and how to render it, falling back on the current environment for values that you don’t specify. For symbol images, the default value of this property is a symbol image configuration object with unspecified values.

You can’t modify this property directly, but you can use withSymbolConfiguration(_:) when you want to create a new image object with a specific set of traits.

