

- ProximityReader
- PaymentCardReaderSession
-  readPaymentCard(\_:eventHandler:) Deprecated

Instance Method

# readPaymentCard(\_:eventHandler:)

Presents a sheet to read a contactless payment card for a purchase or a refund, and returns the encrypted card data.

iOS 15.4–16.0DeprecatediPadOS 15.4–16.0DeprecatedMac Catalyst 17.0–17.0Deprecated

``` source
func readPaymentCard(
    _ request: PaymentCardTransactionRequest,
    eventHandler: ((PaymentCardReaderSession.Event) -> Void)? = nil
) async throws -> PaymentCardReadResult
```

Deprecated

Use PaymentCardReader events instead of eventHandler

## Parameters 

`request`  

The transaction object you provide with the payment amount and currency details.

## Return Value

A PaymentCardReadResult if the read operation was successful.

## Discussion

Call this method as the first step in a financial transaction involving Tap to Pay with iPhone. This method displays a system-provided sheet with instructions on what the person needs to do. This UI remains onscreen until the system reads the person’s card, you cancel the operation, or an error occurs. After the read operation concludes successfully, deliver the returned card information to your payment service provider.

Throws

This method throws a PaymentCardReaderSession.ReadError if a person dismisses the sheet or the sheet fails to appear.

## See Also

### Deprecated

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

enum Event

Optional events you can observe during the card-reading process.

Deprecated

