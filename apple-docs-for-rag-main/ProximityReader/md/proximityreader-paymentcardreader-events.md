

- ProximityReader
- PaymentCardReader
-  events 

Instance Property

# events

A stream of events you receive indicating the activities of the payment card reader.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+

``` source
final let events: AsyncStream
```

## Mentioned in 

Adding support for Tap to Pay on iPhone to your app

## Discussion

When calling prepare(using:), the PaymentCardReader.Event.updateProgress(_:) event will indicate the completion percentage of the configuration. When reading cards with PaymentCardReaderSession, the raised events will indicate the current state of the card-reading process.

## See Also

### Observing reader events

enum Event

An event you receive indicating the state or activity of the payment card reader.

