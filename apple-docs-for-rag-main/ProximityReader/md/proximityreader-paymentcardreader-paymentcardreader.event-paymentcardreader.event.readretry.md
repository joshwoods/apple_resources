

- ProximityReader
- PaymentCardReader
- PaymentCardReader.Event
-  PaymentCardReader.Event.readRetry 

Case

# PaymentCardReader.Event.readRetry

An event that indicates the UI triggered a retry.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+

``` source
case readRetry
```

## See Also

### Getting the event type

case cardDetected

An event that indicates the reader detected the presence of a card.

case pinEntryCompleted

An event that indicates the reader captured the card PIN successfully.

case pinEntryRequested

An event that indicates the reader requested the card PIN.

case readCancelled

An event that indicates the cancellation of the operation.

case readCompleted

An event that indicates the reader completed the reading process.

case readNotCompleted

An event that indicates the read operation didn’t finish.

case readyForTap

An event that indicates the reader is ready for someone to move their card within range of the iPhone.

case removeCard

An event that indicates the consumer can move the card away from the device.

case updateProgress(Int)

The current update progress, specified as an integer value from 1 to 100.

case userInterfaceDismissed

An event that indicates the UI has been closed.

case notReady

A reader that is not ready to perform transactions.

