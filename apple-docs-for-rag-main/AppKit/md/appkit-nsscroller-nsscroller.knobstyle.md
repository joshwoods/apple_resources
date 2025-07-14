

- AppKit
- NSScroller
-  NSScroller.KnobStyle 

Enumeration

# NSScroller.KnobStyle

Specify different knob styles.

macOS 10.7+

``` source
enum KnobStyle
```

## Topics

### Constants

case `default`

Specifies a dark knob with a light border.

case dark

Specifies a dark knob.

case light

Specifies a light knob.

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

### Constants

enum Style

Constants to specify the scroller style.

enum Part

These constants specify the different parts of the scroller:

enum Arrow

These constants describe the two scroller buttons and are used by drawArrow(_:highlight:).

Deprecated

enum ArrowPosition

These constants specify where the scroller’s buttons appear and are used by the arrowsPosition property.

Deprecated

enum UsableParts

These constants specify which parts of the scroller are visible.

