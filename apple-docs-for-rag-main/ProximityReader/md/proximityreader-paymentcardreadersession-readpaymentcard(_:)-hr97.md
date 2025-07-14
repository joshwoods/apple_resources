

- ProximityReader
- PaymentCardReaderSession
-  readPaymentCard(\_:) 

Instance Method

# readPaymentCard(\_:)

Presents a sheet to verify a contactless payment card, and returns the card data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+

``` source
func readPaymentCard(_ request: PaymentCardVerificationRequest) async throws -> PaymentCardReadResult
```

## Parameters 

`request`  

The object that contains the reason for the verification request. For example, you might verify the card supports a specific currency.

## Return Value

A PaymentCardReadResult if the read operation was successful.

## Discussion

Call this method when you want to verify someone’s card with your payment provider. When you call this method, the system displays UI with instructions on what the person needs to do. This UI remains onscreen until the system reads the person’s card, you cancel the operation, or an error occurs.

Throws

This method throws a PaymentCardReaderSession.ReadError if a person dismisses the sheet or the sheet fails to appear.

## See Also

### Reading a payment card

func readPaymentCard(PaymentCardTransactionRequest) async throws -> PaymentCardReadResult

Presents a sheet to read a contactless payment card for a purchase or a refund, and returns the encrypted card data.

