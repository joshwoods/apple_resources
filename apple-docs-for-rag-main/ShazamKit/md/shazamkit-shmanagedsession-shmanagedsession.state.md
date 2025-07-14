

- ShazamKit
- SHManagedSession
-  SHManagedSession.State 

Enumeration

# SHManagedSession.State

The state of a managed session.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@frozen
enum State
```

## Topics

### Getting session states

case idle

The session isn’t recording or making a match attempt.

case matching

The session is recording and making at least one match attempt.

case prerecording

The session has the resources it needs for matching and is prerecording.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Getting the session state

var state: SHManagedSession.State

The current state of the managed session.

