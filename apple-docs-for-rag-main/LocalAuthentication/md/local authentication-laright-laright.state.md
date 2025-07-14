

- Local Authentication
- LARight
-  LARight.State 

Enumeration

# LARight.State

The possible states for a right during authorization.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
enum State
```

## Overview

You can use key-value observation and the Combine framework to observe the authorization state of an LARight instance:

```
let right = LARight()
let cancellable = right
    .publisher(for: \.state)
    .sink { _ in
        print("Right updated to \(right.state)")
    }

try await right.authorize(localizedReason: "Access sandcastle competition designs")
```

## Topics

### Authorization states

case authorizing

The authorization is in progress but not completed.

case authorized

The authorization completed successfully.

case notAuthorized

The authorization failed.

case unknown

The authorization is in an unknown state.

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

### Authentication and access

class LARight

A grouped set of requirements that gate access to a resource or operation.

class LAContext

A mechanism for evaluating authentication policies and access controls.

