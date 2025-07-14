

- UIKit
- UIListContentConfiguration
- UIListContentConfiguration.TextProperties
-  adjustsFontSizeToFitWidth 

Instance Property

# adjustsFontSizeToFitWidth

A Boolean value that determines whether the configuration automatically adjusts the font size of the text when necessary to fit in the available width.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var adjustsFontSizeToFitWidth: Bool { get set }
```

## See Also

### Configuring text properties

var font: UIFont

The font for the text.

var color: UIColor

The color of the text.

var colorTransformer: UIConfigurationColorTransformer?

The color transformer for resolving the text color.

func resolvedColor() -> UIColor

Generates the resolved color for the specified color, using the text color and color transformer.

var alignment: UIListContentConfiguration.TextProperties.TextAlignment

The alignment for the text.

var lineBreakMode: NSLineBreakMode

The line break mode to use for the text.

var numberOfLines: Int

The maximum number of lines for the text.

var minimumScaleFactor: CGFloat

The smallest multiplier for the font size that the configuration uses to make the text fit.

var allowsDefaultTighteningForTruncation: Bool

A Boolean value that determines whether the configuration tightens the text before truncating.

var adjustsFontForContentSizeCategory: Bool

A Boolean value that determines whether the configuration automatically updates the font when the content size category changes.

enum TextAlignment

Constants that specify the visual alignment of the text.

var transform: UIListContentConfiguration.TextProperties.TextTransform

The transform to apply to the text.

enum TextTransform

Constants that specify the transform to apply to the text.

var showsExpansionTextWhenTruncated: Bool

A Boolean value that determines whether the full text displays when the pointer hovers over the truncated text.

