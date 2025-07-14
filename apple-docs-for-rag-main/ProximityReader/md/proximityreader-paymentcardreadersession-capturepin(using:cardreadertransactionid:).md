

- ProximityReader
- PaymentCardReaderSession
-  capturePIN(using:cardReaderTransactionID:) 

Instance Method

# capturePIN(using:cardReaderTransactionID:)

Presents a sheet to capture the PIN when required by the payment card issuer, and returns the previously encrypted card data including newly captured PIN data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+

``` source
func capturePIN(
    using token: PaymentCardReaderSession.PINToken,
    cardReaderTransactionID: String
) async throws -> PaymentCardReadResult
```

## Parameters 

`token`  

Valid and signed PIN token from a participating payment service provider.

`cardReaderTransactionID`  

The id of the previous read.

## Return Value

PaymentCardReadResult if the PIN was successfully captured.

## Mentioned in 

Adding support for Tap to Pay on iPhone to your app

## Discussion

Call this method when the payment card issuer requests a PIN for the current transaction. When you call this method, the system displays UI with instructions on what the person needs to do. This UI remains onscreen until the system reads the person’s PIN, you cancel the operation, or an error occurs.

Important

The encrypted payment card data are only kept 55 seconds after previous read if the PIN was not requested by the card. After this delay, this method will return PaymentCardReaderSession.ReadError.pinEntryFailed

Throws

This method throws a PaymentCardReaderSession.ReadError if a person dismisses the sheet or the sheet fails to appear.

## See Also

### Requesting the PIN

struct PINToken

A secure PIN token that you receive from your participating payment service provider.

