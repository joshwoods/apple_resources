

- UIKit
-  UIVibrancyEffectStyle 

Enumeration

# UIVibrancyEffectStyle

Constants for the vibrancy styles.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum UIVibrancyEffectStyle
```

## Topics

### Label styles

case label

A style for labels containing primary content.

case secondaryLabel

A style for labels containing secondary content.

case tertiaryLabel

A style for labels containing tertiary content.

case quaternaryLabel

A style for labels containing quaternary content.

### Fill styles

case fill

A style for views with large filled areas containing primary content.

case secondaryFill

A style for views with large filled areas containing secondary content.

case tertiaryFill

A style for views with large filled areas containing tertiary content.

### Separator style

case separator

A style for separator lines.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating a vibrancy effect

init(forBlurEffect: UIBlurEffect, style: UIVibrancyEffectStyle)

Creates a vibrancy effect with the specified blur and style values.

init(blurEffect: UIBlurEffect)

Creates a vibrancy effect for a specific blur effect.

