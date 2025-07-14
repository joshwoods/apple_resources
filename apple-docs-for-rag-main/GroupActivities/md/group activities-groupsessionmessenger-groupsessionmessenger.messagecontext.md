

- Group Activities
- GroupSessionMessenger
-  GroupSessionMessenger.MessageContext 

Structure

# GroupSessionMessenger.MessageContext

A structure that contains additional information about an incoming message, such as which device sent it.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
struct MessageContext
```

## Mentioned in 

Synchronizing data during a SharePlay activity

## Topics

### Getting the initiating participant

var source: Participant

The participant device that sent the message.

## Relationships

### Conforms To

- Sendable

## See Also

### Receiving data from other participants

func messages(of: Data.Type) -> GroupSessionMessenger.Messages&lt;Data>

Returns the asynchronous sequence of messages that contain a generic data object.

func messages&lt;Message>(of: Message.Type) -> GroupSessionMessenger.Messages&lt;Message>

Returns the asynchronous sequence of messages that match the app-specific type.

struct Messages

An asynchronous sequence of messages sent to the session.

