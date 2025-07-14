

- AppKit
- NSScroller
-  NSScroller.UsableParts 

Enumeration

# NSScroller.UsableParts

These constants specify which parts of the scroller are visible.

macOS

``` source
enum UsableParts
```

## Topics

### Constants

case noScrollerParts

Specifies that the scroller has neither a knob nor scroll buttons, only the knob slot.

Deprecated

case onlyScrollerArrows

Specifies that the scroller has only scroll buttons, no knob.

Deprecated

case allScrollerParts

Specifies that the scroller has at least a knob, possibly also scroll buttons.

### Initializers

init?(rawValue: UInt)

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

