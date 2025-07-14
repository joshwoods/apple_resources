

- LiveCommunicationKit
- Conversation
-  Conversation.Event 

Enumeration

# Conversation.Event

Specifies the type of event that has happened.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
enum Event
```

## Topics

### Operators

static func == (Conversation.Event, Conversation.Event) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case conversationConnected(Date)

Informs that system that `Conversation` successfully connected at the given `Date`.

case conversationEnded(Date, Conversation.EndedReason)

Informs that system that `Conversation` ended at the given `Date`, with the given `EndedReason`.

case conversationStartedConnecting(Date)

Informs that system that `Conversation` has started connecting at the given `Date`.

case conversationUpdated(Conversation.Update)

Updates a `Conversation` with the given `Update`.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

