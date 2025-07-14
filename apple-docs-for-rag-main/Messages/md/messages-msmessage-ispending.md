

- Messages
- MSMessage
-  isPending 

Instance Property

# isPending

A Boolean value that indicates whether the message is pending or whether it has been sent or received.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var isPending: Bool { get }
```

## Discussion

Use this property to determine whether an MSMessage instance represents an unsent message—for example, to determine whether the conversation’s selectedMessage property refers to a message in the transcript (false) or to a message in the Messages app’s input field (true).

This property’s value is set based on the following rules:

- This property is set to true when your app calls the insert(_:completionHandler:) method to place the message in the Messages app’s input field.

- It’s set to false when the system calls the didStartSending(_:conversation:) method (either because the user sent the message from the input field or because you called the send(_:completionHandler:) method to send it directly).

- This property is set to false on messages received from other participants.

In other words, the property is true only for the selected method of the active conversation when there’s an MSMessagesAppViewController instance in the Messages app’s input field.

## See Also

### Message Properties

var accessibilityLabel: String?

A localized string that describes the message.

var error: (any Error)?

An error object describing why the system failed to send the message.

var layout: MSMessageLayout?

A layout object that defines the message’s appearance.

var senderParticipantIdentifier: UUID

A UUID identifying the participant that sent the message.

var session: MSSession?

The session that this message belongs to.

var shouldExpire: Bool

A Boolean value that determines whether the message should expire after being read.

var summaryText: String?

A succinct description of the message.

var url: URL?

A URL that encodes data to be transmitted with the message.

