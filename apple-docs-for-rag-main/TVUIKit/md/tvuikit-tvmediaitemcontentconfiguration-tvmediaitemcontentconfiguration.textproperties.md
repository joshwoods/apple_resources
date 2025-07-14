

- TVUIKit
- TVMediaItemContentConfiguration
-  TVMediaItemContentConfiguration.TextProperties 

Structure

# TVMediaItemContentConfiguration.TextProperties

Properties that affect the media item content configuration’s text.

tvOS 15.0+

``` source
struct TextProperties
```

## Topics

### Configuring Text Properties

var font: UIFont

The font for the text.

var color: UIColor

The color of the text.

var transform: TVMediaItemContentConfiguration.TextProperties.TextTransform

The transform to apply to the text before displaying it.

enum TextTransform

Constants that specify the transform to apply to the text.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- Hashable

## See Also

### Customizing Appearance

var textProperties: TVMediaItemContentConfiguration.TextProperties

Properties for configuring the primary text.

var secondaryTextProperties: TVMediaItemContentConfiguration.TextProperties

Properties for configuring the secondary text.

