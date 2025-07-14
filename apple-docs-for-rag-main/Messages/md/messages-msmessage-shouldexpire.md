

- Messages
- MSMessage
-  shouldExpire 

Instance Property

# shouldExpire

A Boolean value that determines whether the message should expire after being read.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
var shouldExpire: Bool { get set }
```

## Discussion

If true, the message should expire after it is read. Expired messages are deleted a short time after being read by the recipient. The recipient may opt to keep the message.

The `shouldExpire` property defaults to false.

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

var summaryText: String?

A succinct description of the message.

var url: URL?

A URL that encodes data to be transmitted with the message.

