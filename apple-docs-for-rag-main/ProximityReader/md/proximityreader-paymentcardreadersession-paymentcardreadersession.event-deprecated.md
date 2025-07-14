

- ProximityReader
- PaymentCardReaderSession
-  PaymentCardReaderSession.Event Deprecated

Enumeration

# PaymentCardReaderSession.Event

Optional events you can observe during the card-reading process.

iOS 15.4–16.0DeprecatediPadOS 15.4–16.0DeprecatedMac Catalyst 17.0–17.0Deprecated

``` source
enum Event
```

Deprecated

Use PaymentCardReader.Event

## Overview

If you supply an event handler when reading a card, the session delivers appropriate events to your handler. Use them to update your UI or perform other app-specific tasks. You can also use them to provide accessibility-related feedback.

## Topics

### Getting the event type

case cardDetected

An event that indicates the reader detected the presence of a card.

case completed

An event that indicates the reader completed the reading process.

case readCancelled

An event that indicates the cancellation of the operation.

case readNotCompleted

An event that indicates the read operation didn’t finish.

case readyForTap

An event that indicates the reader is ready for someone to move their card within range of the iPhone.

case removeCard

An event that indicates the consumer can move the card away from the device.

case retry

An event that indicates the UI triggered a retry.

### Getting the event name

var name: String

The name of the event.

### Operators

static func == (PaymentCardReaderSession.Event, PaymentCardReaderSession.Event) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Deprecated

func readPaymentCard(PaymentCardTransactionRequest, eventHandler: ((PaymentCardReaderSession.Event) -> Void)?) async throws -> PaymentCardReadResult

Presents a sheet to read a contactless payment card for a purchase or a refund, and returns the encrypted card data.

Deprecated

func readPaymentCard(PaymentCardVerificationRequest, eventHandler: ((PaymentCardReaderSession.Event) -> Void)?) async throws -> PaymentCardReadResult

Presents a sheet to verify a contactless payment card, and returns the card data.

Deprecated

func readPaymentCard(PaymentCardTransactionRequest, vasRequest: VASRequest, stopOnVASResult: Bool, eventHandler: ((PaymentCardReaderSession.Event) -> Void)?) async throws -> (PaymentCardReadResult?, VASReadResult?)

Presents a sheet to read both contactless payments and loyalty cards for a purchase or refund, and returns the relevant card data.

Deprecated

func readVAS(VASRequest, eventHandler: ((PaymentCardReaderSession.Event) -> Void)?) async throws -> VASReadResult

Presents a sheet to read a loyalty card for Value Added Services (VAS), and returns the loyalty card data.

Deprecated

let id: String

A unique identifier for this object.

Deprecated

