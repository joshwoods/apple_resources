

- ProximityReader
- PaymentCardReaderSession
-  readPaymentCard(\_:vasRequest:stopOnVASResult:) 

Instance Method

# readPaymentCard(\_:vasRequest:stopOnVASResult:)

Presents a sheet to read both contactless payments and loyalty cards for a purchase or refund, and returns the relevant card data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+

``` source
func readPaymentCard(
    _ request: PaymentCardTransactionRequest,
    vasRequest: VASRequest,
    stopOnVASResult: Bool
) async throws -> (PaymentCardReadResult?, VASReadResult?)
```

## Parameters 

`request`  

The transaction object you provide with the payment amount and currency details.

`vasRequest`  

The object that you use to specify the loyalty card request details, such as the list of supported merchants.

`stopOnVASResult`  

A Boolean that indicates what type of result to return. See the discussion for details of how this parameter affects the return value.

## Return Value

Either PaymentCardReadResult, VASReadResult, or both when the read operation was successful.

## Mentioned in 

Accepting loyalty passes from Wallet

## Discussion

Call this method to read either a contactless payment card or a loyalty card. This method displays a system sheet with instructions on what the person needs to do. The system UI remains onscreen until the system reads the person’s card, you cancel the operation, or an error occurs. If it reads a card successfully, the method returns the card information as a result.

When the `stopOnVasResult` parameter is `true`:

- If the customer taps their loyalty card while the UI is present, the system closes the sheet and returns VASReadResult as a result.

- If the customer taps their payment card while the UI is present, the system closes the sheet and returns PaymentCardReadResult as a result.

When the `stopOnVasResult` parameter is `false`:

- If the customer taps their Apple Pay Wallet, containing both a relevant loyalty card and a payment card, the system closes the sheet and returns both PaymentCardReadResult and VASReadResult as a result.

- If the customer taps their Apple Pay Wallet, containing only a relevant loyalty card, the system closes the sheet and returns VASReadResult as a result.

- If the customer taps their payment card, the system closes the sheet and returns PaymentCardReadResult as a result.

Throws

This method throws a PaymentCardReaderSession.ReadError if a person dismisses the sheet or the sheet fails to appear.

## See Also

### Reading a loyalty card

func readVAS(VASRequest) async throws -> VASReadResult

Presents a sheet to read a loyalty card for Value Added Services (VAS), and returns the loyalty card data.

