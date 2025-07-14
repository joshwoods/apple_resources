

- LiveCommunicationKit
- Conversation
-  Conversation.Update 

Structure

# Conversation.Update

An encapsulation of new, changed, or deleted information about a conversation.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
struct Update
```

## Topics

### Operators

static func == (Conversation.Update, Conversation.Update) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

init(localMember: Handle?, members: Set&lt;Handle>?, activeRemoteMembers: Set&lt;Handle>?, capabilities: Conversation.Capabilities?)

Creates a new `Update`. Note that `nil` value means “no change”.

### Instance Properties

var activeRemoteMembers: Set&lt;Handle>?

All active remote members.

var capabilities: Conversation.Capabilities?

Functionality that the conversation supports once the `Update` is applied.

var hashValue: Int

The hash value.

var localMember: Handle?

The local member in the conversation.

var members: Set&lt;Handle>?

All members of the conversation, including inactive (but invited) remote members.

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

