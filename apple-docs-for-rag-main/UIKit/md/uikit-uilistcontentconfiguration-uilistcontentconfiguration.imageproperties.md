

- UIKit
- UIListContentConfiguration
-  UIListContentConfiguration.ImageProperties 

Structure

# UIListContentConfiguration.ImageProperties

Properties that affect the list content configuration’s image.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
struct ImageProperties
```

## Topics

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

static let standardDimension: CGFloat

The system standard layout dimension for reserved layout size.

var accessibilityIgnoresInvertColors: Bool

A Boolean value that determines whether the image inverts its colors when the user turns on the Invert Colors accessibility setting.

### Instance Properties

var strokeColor: UIColor?

var strokeColorTransformer: UIConfigurationColorTransformer?

var strokeWidth: CGFloat

### Instance Methods

func resolvedStrokeColor(for: UIColor) -> UIColor

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- Hashable

## See Also

### Customizing appearance

var imageProperties: UIListContentConfiguration.ImageProperties

Properties for configuring the image.

var textProperties: UIListContentConfiguration.TextProperties

Properties for configuring the primary text.

var secondaryTextProperties: UIListContentConfiguration.TextProperties

Properties for configuring the secondary text.

struct TextProperties

Properties that affect the list content configuration’s text.

