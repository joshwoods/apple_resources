

- ProximityReader
- PaymentCardReaderSession
-  readPaymentCard(\_:eventHandler:) Deprecated

Instance Method

# readPaymentCard(\_:eventHandler:)

Presents a sheet to verify a contactless payment card, and returns the card data.

iOS 15.4–16.0DeprecatediPadOS 15.4–16.0DeprecatedMac Catalyst 17.0–17.0Deprecated

``` source
func readPaymentCard(
    _ request: PaymentCardVerificationRequest,
    eventHandler: ((PaymentCardReaderSession.Event) -> Void)? = nil
) async throws -> PaymentCardReadResult
```

Deprecated

Use PaymentCardReader events instead of eventHandler

## Parameters 

`request`  

The object that contains the reason for the verification request. For example, you might verify the card supports a specific currency.

`eventHandler`  

A handler you use to receive request-related updates while the system has control of the screen. The handler has no return value and takes a PaymentCardReaderSession.Event as a parameter. Use the event parameter to determine what happened.

## Return Value

A PaymentCardReadResult if the read operation was successful.

## Discussion

Call this method when you want to verify someone’s card with your payment provider. When you call this method, the system displays UI with instructions on what the person needs to do. This UI remains onscreen until the system reads the person’s card, you cancel the operation, or an error occurs.

Throws

This method throws a PaymentCardReaderSession.ReadError if a person dismisses the sheet or the sheet fails to appear.

## See Also

### Deprecated

func readPaymentCard(PaymentCardTransactionRequest, eventHandler: ((PaymentCardReaderSession.Event) -> Void)?) async throws -> PaymentCardReadResult

Presents a sheet to read a contactless payment card for a purchase or a refund, and returns the encrypted card data.

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

enum Event

Optional events you can observe during the card-reading process.

Deprecated

