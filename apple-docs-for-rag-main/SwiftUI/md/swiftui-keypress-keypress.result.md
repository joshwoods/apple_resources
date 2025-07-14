

- SwiftUI
- KeyPress
-  KeyPress.Result 

Enumeration

# KeyPress.Result

A result value returned from a key-press action that indicates whether the action consumed the event.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
enum Result
```

## Topics

### Getting the result

case handled

The action consumed the event, preventing dispatch from continuing.

case ignored

The action ignored the event, allowing dispatch to continue.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

