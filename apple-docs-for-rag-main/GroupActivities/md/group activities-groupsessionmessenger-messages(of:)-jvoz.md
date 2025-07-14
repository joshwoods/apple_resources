

- Group Activities
- GroupSessionMessenger
-  messages(of:) 

Instance Method

# messages(of:)

Returns the asynchronous sequence of messages that match the app-specific type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
final func messages(of type: Message.Type) -> GroupSessionMessenger.Messages where Message : Decodable, Message : Encodable
```

## Parameters 

`type`  

The class of the custom type you use to package the message contents.

## Discussion

Call this method to receive the messages that other participants send to the group. This method returns a GroupSessionMessenger.Messages structure, which conforms to the `AsyncSequence` protocol. This sequence contains all, some, or none of the messages sent over time. You retrieve messages by iterating over them using an asynchronous `for`-`in` loop, as shown in the following example:

```
let sessionMessenger = GroupSessionMessenger(session: groupSession)

async {
    for await move in sessionMessenger.messages(of: TicTacToe.Move.self) {
        self.board.addMove(move)
    }
}
```

## See Also

### Receiving data from other participants

func messages(of: Data.Type) -> GroupSessionMessenger.Messages&lt;Data>

Returns the asynchronous sequence of messages that contain a generic data object.

struct Messages

An asynchronous sequence of messages sent to the session.

struct MessageContext

A structure that contains additional information about an incoming message, such as which device sent it.

