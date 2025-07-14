

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  automaticReloadPaymentRequest 

Instance Property

# automaticReloadPaymentRequest

An optional request to set up an automatic reload payment, such as a store card top-up.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var automaticReloadPaymentRequest: PKAutomaticReloadPaymentRequest? { get set }
```

## Discussion

Set this property by assigning it to an instance of PKAutomaticReloadPaymentRequest to indicate that the payment request is for an automatic reload payment.

Apple Pay issues an Apple Pay Merchant Token if the user’s payment network supports merchant-specific payment tokens. Otherwise, Apple Pay issues a device token for the payment request.

Important

You can’t use this property with multiTokenContexts or recurringPaymentRequest or deferredPaymentRequest properties. Simultaneous use of these properties results in a runtime error and cancels the payment request.

## See Also

### Requesting recurring, automatic, and deferred payments

var recurringPaymentRequest: PKRecurringPaymentRequest?

An optional request to set up a recurring payment, typically a subscription.

class PKRecurringPaymentRequest

A class that represents a request to set up a recurring payment, typically a subscription.

class PKAutomaticReloadPaymentRequest

A class that represents a request to set up an automatic reload payment, such as a store card top-up or a prepaid account.

var deferredPaymentRequest: PKDeferredPaymentRequest?

A request to set up a deferred payment, such as a hotel booking or a pre-order.

class PKDeferredPaymentRequest

An object that represents a request to set up a deferred payment, such as a hotel booking or a pre-order.

