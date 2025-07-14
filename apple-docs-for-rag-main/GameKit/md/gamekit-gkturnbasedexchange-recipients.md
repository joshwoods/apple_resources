

- GameKit
- GKTurnBasedExchange
-  recipients 

Instance Property

# recipients

The participants who receives the exchange request.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var recipients: [GKTurnBasedParticipant] { get }
```

## See Also

### Retrieving Exchange Details

var exchangeID: String

The identifier for the exchange request.

var sender: GKTurnBasedParticipant

The participant who sends the exchange request to recipients.

var data: Data?

The game-specific exchange data that GameKit sends to participants.

var message: String?

A localized message from the sender to the recipients of an exchange request.

var sendDate: Date

The date that the sender initiates the exchange request.

var timeoutDate: Date?

The date that the recipients must reply by before the exchange request times out.

