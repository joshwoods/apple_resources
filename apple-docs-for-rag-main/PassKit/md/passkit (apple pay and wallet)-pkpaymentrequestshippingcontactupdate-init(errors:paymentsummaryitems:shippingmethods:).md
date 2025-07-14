

- PassKit (Apple Pay and Wallet)
- PKPaymentRequestShippingContactUpdate
-  init(errors:paymentSummaryItems:shippingMethods:) 

Initializer

# init(errors:paymentSummaryItems:shippingMethods:)

Creates a shipping contact update with your specified payment summary items and shipping methods.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
init(
    errors: [any Error]?,
    paymentSummaryItems: [PKPaymentSummaryItem],
    shippingMethods: [PKShippingMethod]
)
```

## Parameters 

`errors`  

An array of errors in the shipping contact information that the user must resolve.

`paymentSummaryItems`  

An array of summary items that include any changes due to fees or credit card surcharges associated with the payment method.

`shippingMethods`  

An array of shipping methods.

## Discussion

Use the `errors` array to specify any errors in the shipping method that the user must resolve. For more information on creating user errors, see PKPaymentError.

