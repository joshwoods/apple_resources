

- UIKit
- UIImage
- UIImage.SymbolConfiguration
-  preferringMonochrome() 

Type Method

# preferringMonochrome()

Creates a color configuration that specifies that the symbol image uses its monochrome variant.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
class func preferringMonochrome() -> Self
```

## Return Value

A symbol configuration that acquires the monochrome variant of a symbol.

## Mentioned in 

Configuring and displaying symbol images in your UI

## See Also

### Creating a color configuration

convenience init(hierarchicalColor: UIColor)

Creates a color configuration with a color scheme that originates from one color.

convenience init(paletteColors: [UIColor])

Creates a color configuration with a color scheme from a palette of multiple colors.

class func preferringMulticolor() -> Self

Creates a color configuration that specifies that the symbol image uses its multicolor variant, if one exists.

