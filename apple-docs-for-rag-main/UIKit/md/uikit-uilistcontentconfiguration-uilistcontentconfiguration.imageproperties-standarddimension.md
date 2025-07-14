

- UIKit
- UIListContentConfiguration
- UIListContentConfiguration.ImageProperties
-  standardDimension 

Type Property

# standardDimension

The system standard layout dimension for reserved layout size.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
static let standardDimension: CGFloat
```

## Discussion

Setting the reservedLayoutSize width or height to this constant results in using the system standard value for a symbol image for that dimension, even when the image is not a symbol image.

## See Also

### Configuring image properties

var preferredSymbolConfiguration: UIImage.SymbolConfiguration?

The symbol configuration to use.

var tintColor: UIColor?

The tint color to apply to the image view.

var tintColorTransformer: UIConfigurationColorTransformer?

The color transformer for resolving the tint color.

func resolvedTintColor(for: UIColor) -> UIColor

Generates the resolved tint color for the specified tint color, using the tint color and color transformer.

var cornerRadius: CGFloat

The preferred corner radius, using a continuous corner curve, for the image.

var maximumSize: CGSize

The maximum size for the image.

var reservedLayoutSize: CGSize

The layout size that the system reserves for the image, and then centers the image within.

var accessibilityIgnoresInvertColors: Bool

A Boolean value that determines whether the image inverts its colors when the user turns on the Invert Colors accessibility setting.

