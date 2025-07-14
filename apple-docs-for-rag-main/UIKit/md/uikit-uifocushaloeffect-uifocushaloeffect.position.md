

- UIKit
- UIFocusHaloEffect
-  UIFocusHaloEffect.Position 

Enumeration

# UIFocusHaloEffect.Position

Constants that describe positions for drawing the halo focus effect.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
enum Position
```

## Topics

### Constants

case automatic

A constant that automatically chooses a position for drawing the halo effect depending on the focus item and its containing view hierarchy.

case outside

A constant that draws the halo effect around the shape.

case inside

A constant that draws the halo effect inside the shape.

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

### Focus effects

class UIFocusEffect

The base class for defining a visual focus effect.

class UIFocusHaloEffect

A visual focus effect that draws a halo around the focus item.

