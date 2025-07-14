

- GameKit
-  GKTurnBasedExchangeStatus 

Enumeration

# GKTurnBasedExchangeStatus

The status of an exchange or reply.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
enum GKTurnBasedExchangeStatus
```

## Topics

### Statuses

case unknown

The state of the exchange request is unknown.

case active

GameKit sent the exchange request to recipients but not all recipients replied.

case complete

All recipients of the exchange request replied.

case resolved

The current participant saved the exchange request.

case canceled

The sender canceled the exchange request.

### Initializers

init?(rawValue: Int8)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Replying to Exchange Requests

func reply(withLocalizableMessageKey: String, arguments: [String], data: Data, completionHandler: (((any Error)?) -> Void)?)

Replies to an exchange request on behalf of a recipient.

var replies: [GKTurnBasedExchangeReply]?

The replies from recipients of the exchange request.

var status: GKTurnBasedExchangeStatus

The status of the exchange request.

var completionDate: Date?

The date when all recipients of the exchange request reply.

