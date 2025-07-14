

- AppKit
- NSScroller
-  NSScroller.Part 

Enumeration

# NSScroller.Part

These constants specify the different parts of the scroller:

macOS

``` source
enum Part
```

## Topics

### Constants

case knob

Directly to the scroller’s value, as given by floatValue.

case knobSlot

Directly to the scroller’s value, as given by floatValue.

case decrementLine

Up or left by a small amount.

Deprecated

case decrementPage

Up or left by a large amount.

case incrementLine

Down or right by a small amount.

Deprecated

case incrementPage

Down or right by a large amount.

case noPart

Don’t scroll at all.

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

enum Arrow

These constants describe the two scroller buttons and are used by drawArrow(_:highlight:).

Deprecated

enum ArrowPosition

These constants specify where the scroller’s buttons appear and are used by the arrowsPosition property.

Deprecated

enum UsableParts

These constants specify which parts of the scroller are visible.

