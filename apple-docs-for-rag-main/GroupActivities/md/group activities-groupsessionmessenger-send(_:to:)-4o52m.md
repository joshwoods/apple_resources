

- Group Activities
- GroupSessionMessenger
-  send(\_:to:) 

Instance Method

# send(\_:to:)

Sends a standard data object asynchronously to other participants in the group session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
final func send(
    _ value: Data,
    to participants: Participants = .all
) async throws
```

## Parameters 

`participants`  

The recipients of the message. The default value of this parameter is the set of all active participants in the session. Use the Participants.only(_:) option to specify a subset of participants.

## Discussion

Use this method to send data with a standard data object. Your app is responsible for decoding and using the data it receives.

## See Also

### Sending data to the group

func send&lt;Message>(Message, to: Participants) async throws

Sends a custom type asynchronously to other participants in the group session.

func send(Data, to: Participants, completion: ((any Error)?) -> Void)

Sends a standard data object to other participants in the group session.

func send&lt;Message>(Message, to: Participants, completion: ((any Error)?) -> Void)

Sends a custom type to other participants in the group session.

enum Participants

The set of participants to include in messages.

