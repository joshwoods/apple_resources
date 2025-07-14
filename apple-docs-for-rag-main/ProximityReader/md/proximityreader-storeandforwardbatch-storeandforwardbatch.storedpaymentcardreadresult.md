

- ProximityReader
- StoreAndForwardBatch
-  StoreAndForwardBatch.StoredPaymentCardReadResult 

Structure

# StoreAndForwardBatch.StoredPaymentCardReadResult

A result structure that represents each payment the framework read using a Store and Forward session.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
struct StoredPaymentCardReadResult
```

## Topics

### Instance Properties

let generalCardData: String

A Base64-encoded string that contains general cardholder and terminal data in tag-length-value (TLV) format.

let id: String

The unique identifier for the payment.

let paymentCardData: String

A Base64-encoded string that contains the encrypted payment information to send to your payment provider.

let signature: String

The signature, as a Base64-encoded string, that guarantees the integrity of the payment

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

## Relationships

### Conforms To

- Encodable
- Identifiable
- Sendable

