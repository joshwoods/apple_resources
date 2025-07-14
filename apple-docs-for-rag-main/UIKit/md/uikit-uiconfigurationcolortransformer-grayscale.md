

- UIKit
- UIConfigurationColorTransformer
-  grayscale 

Type Property

# grayscale

Creates a color transformer that generates a grayscale version of the color.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
static let grayscale: UIConfigurationColorTransformer
```

## See Also

### Creating a color transformer

init((UIColor) -> UIColor)

Creates a color transformer with the specified closure.

static let preferredTint: UIConfigurationColorTransformer

A color transformer that returns the preferred system accent color.

static let monochromeTint: UIConfigurationColorTransformer

A color transformer that returns the color with a monochrome tint.

