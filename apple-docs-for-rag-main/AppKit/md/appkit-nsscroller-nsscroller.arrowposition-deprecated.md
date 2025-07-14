

- AppKit
- NSScroller
-  NSScroller.ArrowPosition Deprecated

Enumeration

# NSScroller.ArrowPosition

These constants specify where the scroller’s buttons appear and are used by the arrowsPosition property.

macOS 10.0–10.14Deprecated

``` source
enum ArrowPosition
```

Deprecated

Scroller arrows are not used anymore.

## Topics

### Constants

case scrollerArrowsMaxEnd

Buttons at bottom or right. This constant has been deprecated.

case scrollerArrowsMinEnd

Buttons at top or left. This has been deprecated.

static var scrollerArrowsDefaultSetting: NSScroller.ArrowPosition

Buttons are displayed according to the system-wide appearance preferences.

case scrollerArrowsNone

No buttons.

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

enum UsableParts

These constants specify which parts of the scroller are visible.

