

- ProximityReader
- PaymentCardReaderSession
-  readVAS(\_:eventHandler:) Deprecated

Instance Method

# readVAS(\_:eventHandler:)

Presents a sheet to read a loyalty card for Value Added Services (VAS), and returns the loyalty card data.

iOS 15.4–16.0DeprecatediPadOS 15.4–16.0DeprecatedMac Catalyst 17.0–17.0Deprecated

``` source
func readVAS(
    _ request: VASRequest,
    eventHandler: ((PaymentCardReaderSession.Event) -> Void)? = nil
) async throws -> VASReadResult
```

Deprecated

Use PaymentCardReader events instead of eventHandler

## Parameters 

`request`  

The object that you use to specify the request details, such as the list of supported merchants.

`eventHandler`  

A handler you use to receive request-related updates. The handler has no return value and takes a PaymentCardReaderSession.Event as a parameter. Use the event parameter to determine what happened.

## Return Value

A VASReadResult if the read operation was successful.

## Discussion

Call this method to read the data from a loyalty card. When you call this method, the system displays UI with instructions on what the person needs to do. This UI remains onscreen until the system reads the person’s card, you cancel the operation, or an error occurs.

Throws

This method throws a PaymentCardReaderSession.ReadError if a person dismisses the sheet or the sheet fails to appear.

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

let id: String

A unique identifier for this object.

Deprecated

enum Event

Optional events you can observe during the card-reading process.

Deprecated

