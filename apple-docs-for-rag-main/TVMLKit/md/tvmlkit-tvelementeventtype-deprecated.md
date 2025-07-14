

- TVMLKit
-  TVElementEventType Deprecated

Enumeration

# TVElementEventType

The type of event that has been dispatched.

tvOS 9.0–18.0Deprecated

``` source
enum TVElementEventType
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Enumeration Cases

case change

A change event has been dispatched.

case highlight

A highlight event has been dispatched.

case holdSelect

A hold event has been dispatched.

case play

A play event has been dispatched.

case select

A select event has been dispatched.

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

### Dispatching Events

func dispatchEvent(type: TVElementEventType, canBubble: Bool, cancellable: Bool, extraInfo: [String : Any]?, completion: ((Bool, Bool) -> Void)?)

Dispatches an event of a specific type to the JavaScript file.

Deprecated

func dispatchEvent(name: String, canBubble: Bool, cancellable: Bool, extraInfo: [String : Any]?, completion: ((Bool, Bool) -> Void)?)

Dispatches a custom-named event.

Deprecated

