

- LiveCommunicationKit
- ConversationAction
-  ConversationAction.State 

Enumeration

# ConversationAction.State

Represents the current state of a `ConversationAction`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
enum State
```

## Topics

### Operators

static func == (ConversationAction.State, ConversationAction.State) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case complete

The action completed successfully.

case failed(reason: String)

The action failed to complete successfully.

case idle

The action has been created, but has not started executing.

case running

The action is currently being executed.

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

