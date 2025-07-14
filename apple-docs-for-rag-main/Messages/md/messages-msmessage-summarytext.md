

- Messages
- MSMessage
-  summaryText 

Instance Property

# summaryText

A succinct description of the message.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
var summaryText: String? { get set }
```

## Discussion

This property defaults to `nil`.

Set the summary text when you create a message that is associated with a session. When a subsequent message is sent using the same session, the Messages app uses this text to create a summary in the transcript. If the summary text is `nil`, the system provides a default description for the message so that the message history is preserved.

## See Also

### Message Properties

var accessibilityLabel: String?

A localized string that describes the message.

var error: (any Error)?

An error object describing why the system failed to send the message.

var isPending: Bool

A Boolean value that indicates whether the message is pending or whether it has been sent or received.

var layout: MSMessageLayout?

A layout object that defines the message’s appearance.

var senderParticipantIdentifier: UUID

A UUID identifying the participant that sent the message.

var session: MSSession?

The session that this message belongs to.

var shouldExpire: Bool

A Boolean value that determines whether the message should expire after being read.

var url: URL?

A URL that encodes data to be transmitted with the message.

