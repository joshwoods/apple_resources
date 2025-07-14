

- UIKit
- UIConfigurationColorTransformer
-  init(\_:) 

Initializer

# init(\_:)

Creates a color transformer with the specified closure.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
init(_ transform: @escaping (UIColor) -> UIColor)
```

## See Also

### Creating a color transformer

static let grayscale: UIConfigurationColorTransformer

Creates a color transformer that generates a grayscale version of the color.

static let preferredTint: UIConfigurationColorTransformer

A color transformer that returns the preferred system accent color.

static let monochromeTint: UIConfigurationColorTransformer

A color transformer that returns the color with a monochrome tint.

