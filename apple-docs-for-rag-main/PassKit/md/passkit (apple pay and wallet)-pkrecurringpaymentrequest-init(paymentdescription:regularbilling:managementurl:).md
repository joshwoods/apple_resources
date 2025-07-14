

- PassKit (Apple Pay and Wallet)
- PKRecurringPaymentRequest
-  init(paymentDescription:regularBilling:managementURL:) 

Initializer

# init(paymentDescription:regularBilling:managementURL:)

Create a recurring payment object with a description, regular billing information, and a management URL.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
init(
    paymentDescription: String,
    regularBilling: PKRecurringPaymentSummaryItem,
    managementURL: URL
)
```

## Parameters 

`paymentDescription`  

The description you provide of the recurring payment and that Apple Pay displays to the user in the payment sheet.

`regularBilling`  

The summary item for the recurring payment that includes the payment period and interval.

`managementURL`  

The URL to a web page where the user can update or delete the payment method for the recurring payment.

## Discussion

Important

You must set the recurringPaymentRequest property on a PKPaymentRequest object to use this class to request a recurring payment.

