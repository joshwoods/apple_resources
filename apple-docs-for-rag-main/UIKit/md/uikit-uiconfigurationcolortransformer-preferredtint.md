

- UIKit
- UIConfigurationColorTransformer
-  preferredTint 

Type Property

# preferredTint

A color transformer that returns the preferred system accent color.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
static let preferredTint: UIConfigurationColorTransformer
```

## Discussion

This color transformer returns the original color on platforms without a system accent color, or when the system accent color is set to Multicolor. When the system accent color is set to any other color, this color transformer returns that system accent color.

## See Also

### Creating a color transformer

init((UIColor) -> UIColor)

Creates a color transformer with the specified closure.

static let grayscale: UIConfigurationColorTransformer

Creates a color transformer that generates a grayscale version of the color.

static let monochromeTint: UIConfigurationColorTransformer

A color transformer that returns the color with a monochrome tint.

