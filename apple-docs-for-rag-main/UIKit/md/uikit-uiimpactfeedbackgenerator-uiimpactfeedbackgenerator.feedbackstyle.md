

- UIKit
- UIImpactFeedbackGenerator
-  UIImpactFeedbackGenerator.FeedbackStyle 

Enumeration

# UIImpactFeedbackGenerator.FeedbackStyle

The mass of the objects in the collision simulated by an impact feedback generator object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
enum FeedbackStyle
```

## Topics

### Constants

case heavy

A collision between large, heavy user interface elements.

case light

A collision between small, light user interface elements.

case medium

A collision between moderately sized user interface elements.

case rigid

A collision between user interface elements that are rigid, exhibiting a small amount of compression or elasticity.

case soft

A collision between user interface elements that are soft, exhibiting a large amount of compression or elasticity.

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

### Initializing the feedback generator

convenience init(style: UIImpactFeedbackGenerator.FeedbackStyle, view: UIView)

Creates an impact feedback generator with the specified style and view.

