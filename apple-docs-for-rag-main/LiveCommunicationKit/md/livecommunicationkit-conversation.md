

- LiveCommunicationKit
-  Conversation 

Class

# Conversation

A VoIP conversation.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
final class Conversation
```

## Topics

### Structures

struct Capabilities

Used to configure a `Conversation` as part of a `Conversation.Update`.

struct Update

An encapsulation of new, changed, or deleted information about a conversation.

### Instance Properties

var localMember: Handle?

The handle used to identify the local member to remote members. Only available to the `ConversationProvider` that provided the conversation.

var state: Conversation.State

The current state of the conversation.

var uuid: UUID

The unique identifier for this conversation.

### Enumerations

enum EndedReason

The reason that a `Conversation` ended.

enum Event

Specifies the type of event that has happened.

enum State

Represents the state of a `Conversation` at a given moment in time.

### Default Implementations

CustomDebugStringConvertible Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Observable
- Sendable

