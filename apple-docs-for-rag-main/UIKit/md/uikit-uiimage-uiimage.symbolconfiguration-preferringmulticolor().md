

- UIKit
- UIImage
- UIImage.SymbolConfiguration
-  preferringMulticolor() 

Type Method

# preferringMulticolor()

Creates a color configuration that specifies that the symbol image uses its multicolor variant, if one exists.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class func preferringMulticolor() -> Self
```

## Return Value

A symbol configuration that acquires the multicolor variant of a symbol.

## Discussion

Use this method to acquire the multicolor variant of a symbol, if one exists. This method is the primary approach to retrieving multicolor symbols.

For this color configuration to have an effect, your symbol image must have the following:

- Its renderingMode set to UIImage.RenderingMode.alwaysTemplate or UIImage.RenderingMode.automatic.

- Multicolor annotations. If your symbol doesn’t have multicolor annotations, the resulting image is a monochrome (template) symbol image. If you combine this configuration with a hierarchical or palette color configuration using applying(_:), the resulting symbol uses the multicolor variant, if one exists, and defaults to the hierarchical or palette variant otherwise.

## See Also

### Creating a color configuration

convenience init(hierarchicalColor: UIColor)

Creates a color configuration with a color scheme that originates from one color.

convenience init(paletteColors: [UIColor])

Creates a color configuration with a color scheme from a palette of multiple colors.

class func preferringMonochrome() -> Self

Creates a color configuration that specifies that the symbol image uses its monochrome variant.

