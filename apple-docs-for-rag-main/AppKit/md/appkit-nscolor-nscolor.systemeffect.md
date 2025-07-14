

- AppKit
- NSColor
-  NSColor.SystemEffect 

Enumeration

# NSColor.SystemEffect

Constants for user interactions that change the appearance of a view or control.

macOS 10.14+

``` source
enum SystemEffect
```

## Topics

### Appearances

case none

No additional effects.

case pressed

The color that indicates the item was pressed.

case deepPressed

The color that indicates the item received a deep press.

case disabled

The color that indicates the item is disabled.

case rollover

The color that indicates the mouse rolled over the item.

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

### Applying Specific Appearances to Colors

func withSystemEffect(NSColor.SystemEffect) -> NSColor

Returns a new color object that represents the current color modified to include the specified visual effect.

