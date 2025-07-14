

- UIKit
- UIConfigurationColorTransformer
-  monochromeTint 

Type Property

# monochromeTint

A color transformer that returns the color with a monochrome tint.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
static let monochromeTint: UIConfigurationColorTransformer
```

## Discussion

Use this color transformer to deemphasize a tinted item. The tinted item remains monochrome regardless of the system accent color.

## See Also

### Creating a color transformer

init((UIColor) -> UIColor)

Creates a color transformer with the specified closure.

static let grayscale: UIConfigurationColorTransformer

Creates a color transformer that generates a grayscale version of the color.

static let preferredTint: UIConfigurationColorTransformer

A color transformer that returns the preferred system accent color.

