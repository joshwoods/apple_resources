

- ProximityReader
- PaymentCardReaderSession
- PaymentCardReaderSession.Event
-  PaymentCardReaderSession.Event.readCancelled Deprecated

Case

# PaymentCardReaderSession.Event.readCancelled

An event that indicates the cancellation of the operation.

iOS 15.4–16.0DeprecatediPadOS 15.4–16.0DeprecatedMac Catalyst 17.0–17.0Deprecated

``` source
case readCancelled
```

Deprecated

Use PaymentCardReader.Event

## See Also

### Getting the event type

case cardDetected

An event that indicates the reader detected the presence of a card.

Deprecated

case completed

An event that indicates the reader completed the reading process.

Deprecated

case readNotCompleted

An event that indicates the read operation didn’t finish.

Deprecated

case readyForTap

An event that indicates the reader is ready for someone to move their card within range of the iPhone.

Deprecated

case removeCard

An event that indicates the consumer can move the card away from the device.

Deprecated

case retry

An event that indicates the UI triggered a retry.

Deprecated

