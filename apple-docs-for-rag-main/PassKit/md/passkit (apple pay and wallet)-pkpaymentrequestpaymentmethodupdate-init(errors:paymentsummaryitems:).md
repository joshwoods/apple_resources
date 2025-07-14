

- PassKit (Apple Pay and Wallet)
- PKPaymentRequestPaymentMethodUpdate
-  init(errors:paymentSummaryItems:) 

Initializer

# init(errors:paymentSummaryItems:)

Creates a payment-method update with your specified payment summary items.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
init(
    errors: [any Error]?,
    paymentSummaryItems: [PKPaymentSummaryItem]
)
```

## Parameters 

`errors`  

An array of errors in the selected payment-method that the user must resolve.

`paymentSummaryItems`  

An array of summary items that include any changes due to fees or credit card surcharges associated with the payment method.

## Discussion

Use the `errors` array to specify any errors in the payment method that the user must resolve. For more information on creating user errors, see PKPaymentError.

