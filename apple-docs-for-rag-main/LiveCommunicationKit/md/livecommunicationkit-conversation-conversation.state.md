

- LiveCommunicationKit
- Conversation
-  Conversation.State 

Enumeration

# Conversation.State

Represents the state of a `Conversation` at a given moment in time.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
enum State
```

## Topics

### Enumeration Cases

case idle

The conversation has been registered with the system, but is not yet active.

case joined

Audio/video streams are active and the user is able to engage with remote participants.

case joining

The conversation is being prepared, e.g. audio and video streams are being established.

case leaving

The conversation is being torn down.

case left

The conversation is no longer active and any audio/video sessions have ended.

case paused

Audio and video streams have been paused, but may be resumed.

### Initializers

init?(rawValue: Int)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: Int

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

