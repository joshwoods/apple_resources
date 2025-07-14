

- UIKit
- UIPress
-  UIPress.Phase 

Enumeration

# UIPress.Phase

Constants that represent the phases of a button press.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
enum Phase
```

## Topics

### Constants

case began

A physical button was pressed.

case changed

A button moved, or the force property changed.

case stationary

A button was pressed but hasn’t moved since the previous event.

case ended

A button was released.

case cancelled

The system canceled tracking for the button.

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

enum PressType

Constants that represent buttons that a person can press.

