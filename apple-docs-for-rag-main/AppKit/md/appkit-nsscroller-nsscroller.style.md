

- AppKit
- NSScroller
-  NSScroller.Style 

Enumeration

# NSScroller.Style

Constants to specify the scroller style.

macOS 10.7+

``` source
enum Style
```

## Topics

### Constants

case legacy

Specifies legacy-style scrollers as prior to macOS 10.7.

case overlay

Specifies overlay-style scrollers in macOS 10.7 and later.

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

enum KnobStyle

Specify different knob styles.

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

