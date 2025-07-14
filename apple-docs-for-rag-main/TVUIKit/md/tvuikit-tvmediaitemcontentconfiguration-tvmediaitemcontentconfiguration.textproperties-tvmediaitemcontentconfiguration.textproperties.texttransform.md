

- TVUIKit
- TVMediaItemContentConfiguration
- TVMediaItemContentConfiguration.TextProperties
-  TVMediaItemContentConfiguration.TextProperties.TextTransform 

Enumeration

# TVMediaItemContentConfiguration.TextProperties.TextTransform

Constants that specify the transform to apply to the text.

tvOS 15.0+

``` source
enum TextTransform
```

## Topics

### Text Transforms

case none

An option with no transform.

case capitalized

A transform for displaying the text with the first character capitalized.

case lowercase

A transform for displaying the text in all lowercase characters.

case uppercase

A transform for displaying the text in all uppercase characters.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Customizing Content

var font: UIFont

The font for the badge text.

var color: UIColor

The color of the badge text.

var backgroundColor: UIColor

The background tint color of the badge.

var transform: TVMediaItemContentConfiguration.TextProperties.TextTransform

The transform to apply to the text before displaying it.

