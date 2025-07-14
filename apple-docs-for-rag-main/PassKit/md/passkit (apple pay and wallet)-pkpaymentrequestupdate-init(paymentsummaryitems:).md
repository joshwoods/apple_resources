

- PassKit (Apple Pay and Wallet)
- PKPaymentRequestUpdate
-  init(paymentSummaryItems:) 

Initializer

# init(paymentSummaryItems:)

Creates a payment request update with the specified payment summary items.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
init(paymentSummaryItems: [PKPaymentSummaryItem])
```

## Parameters 

`paymentSummaryItems`  

An array of summary items that include any changes due to fees or credit card surcharges associated with the payment method.

