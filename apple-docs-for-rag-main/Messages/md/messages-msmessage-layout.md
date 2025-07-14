

- Messages
- MSMessage
-  layout 

Instance Property

# layout

A layout object that defines the message’s appearance.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@NSCopying
var layout: MSMessageLayout? { get set }
```

## Discussion

Set this property to a concrete subclass of the abstract MSMessageLayout class.

By default, the `layout` property is set to `nil`.

## See Also

### Message Properties

var accessibilityLabel: String?

A localized string that describes the message.

var error: (any Error)?

An error object describing why the system failed to send the message.

var isPending: Bool

A Boolean value that indicates whether the message is pending or whether it has been sent or received.

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

