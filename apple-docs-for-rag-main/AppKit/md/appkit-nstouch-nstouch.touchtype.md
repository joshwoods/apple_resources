

- AppKit
- NSTouch
-  NSTouch.TouchType 

Enumeration

# NSTouch.TouchType

A bit mask identifying a direct or indirect touch type.

macOS 10.12.2+

``` source
enum TouchType
```

## Topics

### Touch Types

case direct

A direct touch from a user’s finger on a screen.

case indirect

An indirect touch that is not on a screen, like a digitizer touch.

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

### Getting the Touch Type

var type: NSTouch.TouchType

A type of touch from a Touch Bar interaction.

struct TouchTypeMask

A bit mask identifying a direct or indirect touch type.

