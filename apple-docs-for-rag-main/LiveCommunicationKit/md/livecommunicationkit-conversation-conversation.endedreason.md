

- LiveCommunicationKit
- Conversation
-  Conversation.EndedReason 

Enumeration

# Conversation.EndedReason

The reason that a `Conversation` ended.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
enum EndedReason
```

## Topics

### Enumeration Cases

case declinedElsewhere

Another device declined the `Conversation`.

case failed

An error occurred while attempting to service the `Conversation`.

case joinedElsewhere

Another device joined the `Conversation`.

case remoteEnded

The remote party explicitly ended the `Conversation`.

case unanswered

The `Conversation` never started connecting and was never explicitly ended, such as when an outgoing or incoming `Conversation` times out.

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

