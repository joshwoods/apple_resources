

- TipKit
- Tips
-  Tips.InvalidationReason 

Enumeration

# Tips.InvalidationReason

A type that describes why the system permanently invalidated a tip.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum InvalidationReason
```

## Topics

### Enumeration Cases

case actionPerformed

The user performed the action that the tip describes.

case displayCountExceeded

The tip exceeded its maximum display count.

case displayDurationExceeded

The tip exceeded its max display duration.

case tipClosed

The user explicitly closed the tip view while it was displaying.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

