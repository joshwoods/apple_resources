

- SwiftUI
- SequenceGesture
-  SequenceGesture.Value 

Enumeration

# SequenceGesture.Value

The value of a sequence gesture that helps to detect whether the first gesture succeeded, so the second gesture can start.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
enum Value
```

## Topics

### Getting gesture values

case first(First.Value)

The first gesture hasn’t ended.

case second(First.Value, Second.Value?)

The first gesture has ended.

## Relationships

### Conforms To

- Copyable
- Equatable
- Sendable

