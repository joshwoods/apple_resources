

- UIKit
- UIListContentConfiguration
- UIListContentConfiguration.ImageProperties
-  reservedLayoutSize 

Instance Property

# reservedLayoutSize

The layout size that the system reserves for the image, and then centers the image within.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var reservedLayoutSize: CGSize { get set }
```

## Discussion

Use this property to ensure:

- Consistent horizontal alignment for images across adjacent content views, even when the images vary in width.

- Consistent height for content views, even when the images vary in height.

The reserved layout size only affects the amount of space for the image, and its positioning within that space. It doesn’t affect the size of the image.

The default value is CGSizeZero. A width or height of zero means that the system uses the default behavior for that dimension:

- The system centers symbol images inside a predefined reserved layout size that scales with the content size category.

- Nonsymbol images use a reserved layout size equal to the actual size of the displayed image.

At Accessibility Dynamic Type sizes, content views ignore the reserved layout width. Content views ignore the reserved layout height when using the special Accessibility Dynamic Type layout where text wraps around the image.

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

static let standardDimension: CGFloat

The system standard layout dimension for reserved layout size.

var accessibilityIgnoresInvertColors: Bool

A Boolean value that determines whether the image inverts its colors when the user turns on the Invert Colors accessibility setting.

