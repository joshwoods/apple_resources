

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  multiTokenContexts 

Instance Property

# multiTokenContexts

An array of payment token contexts to request multiple payment tokens with one payment token per context.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var multiTokenContexts: [PKPaymentTokenContext] { get set }
```

## Discussion

Use multitoken contexts to indicate payments for multiple merchants. This property is an array of PKPaymentTokenContext objects. The sum of all payment token contexts must be less than or equal to the grand total of the enclosing payment request listed as the last payment summary item, PKPaymentSummaryItem. Otherwise, the request results in a runtime error and cancels the payment request.

Important

You can’t use this property with recurringPaymentRequest or automaticReloadPaymentRequest properties. Simultaneous use of these properties results in a runtime error and cancels the payment request.

## See Also

### Requesting multitoken or multimerchant payments

class PKPaymentTokenContext

A class that defines the context for a single payment token in a payment request for multimerchant payments.

