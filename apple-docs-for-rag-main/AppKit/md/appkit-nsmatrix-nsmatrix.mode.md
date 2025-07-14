

- AppKit
- NSMatrix
-  NSMatrix.Mode 

Enumeration

# NSMatrix.Mode

These constants determine how NSCell objects behave when an NSMatrix object is tracking the mouse.

macOS

``` source
enum Mode
```

## Topics

### Constants

case trackModeMatrix

The NSCell objects are asked to track the mouse with trackMouse(with:in:of:untilMouseUp:) whenever the cursor is inside their bounds. No highlighting is performed.

case highlightModeMatrix

An NSCell is highlighted before it’s asked to track the mouse, then unhighlighted when it’s done tracking.

case radioModeMatrix

Selects no more than one NSCell at a time.

case listModeMatrix

NSCell objects are highlighted, but don’t track the mouse.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

