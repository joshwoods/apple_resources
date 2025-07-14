

- Group Activities
-  Participants 

Enumeration

# Participants

The set of participants to include in messages.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum Participants
```

## Topics

### Getting the set of participants

case all

The set of all participants.

case only(Set&lt;Participant>)

A custom subset of participants.

static func only(Participant) -> Participants

Returns a set containing the specified participant.

## See Also

### Sending data to the group

func send(Data, to: Participants) async throws

Sends a standard data object asynchronously to other participants in the group session.

func send&lt;Message>(Message, to: Participants) async throws

Sends a custom type asynchronously to other participants in the group session.

func send(Data, to: Participants, completion: ((any Error)?) -> Void)

Sends a standard data object to other participants in the group session.

func send&lt;Message>(Message, to: Participants, completion: ((any Error)?) -> Void)

Sends a custom type to other participants in the group session.

