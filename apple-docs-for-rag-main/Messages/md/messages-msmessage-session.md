

- Messages
- MSMessage
-  session 

Instance Property

# session

The session that this message belongs to.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
var session: MSSession? { get }
```

## Discussion

The `session` property is set to the session object passed to the init(session:) initializer; otherwise, it is set to `nil`.

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

var shouldExpire: Bool

A Boolean value that determines whether the message should expire after being read.

var summaryText: String?

A succinct description of the message.

var url: URL?

A URL that encodes data to be transmitted with the message.

