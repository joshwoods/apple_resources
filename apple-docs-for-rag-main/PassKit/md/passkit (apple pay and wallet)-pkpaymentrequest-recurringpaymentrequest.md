

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  recurringPaymentRequest 

Instance Property

# recurringPaymentRequest

An optional request to set up a recurring payment, typically a subscription.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var recurringPaymentRequest: PKRecurringPaymentRequest? { get set }
```

## Discussion

Apple Pay issues an Apple Pay Merchant Token if the user’s payment network supports merchant-specific payment tokens. Otherwise, Apple Pay issues a device token for the payment request.

This property is optional. Set this property by assigning it to an instance of PKRecurringPaymentRequest.

Important

You can’t use this property with multiTokenContexts or automaticReloadPaymentRequest properties. Simultaneous use of these properties results in a runtime error and cancels the payment request. Simultaneous use of these properties results in a runtime error and cancels the payment request.

## See Also

### Requesting recurring, automatic, and deferred payments

class PKRecurringPaymentRequest

A class that represents a request to set up a recurring payment, typically a subscription.

var automaticReloadPaymentRequest: PKAutomaticReloadPaymentRequest?

An optional request to set up an automatic reload payment, such as a store card top-up.

class PKAutomaticReloadPaymentRequest

A class that represents a request to set up an automatic reload payment, such as a store card top-up or a prepaid account.

var deferredPaymentRequest: PKDeferredPaymentRequest?

A request to set up a deferred payment, such as a hotel booking or a pre-order.

class PKDeferredPaymentRequest

An object that represents a request to set up a deferred payment, such as a hotel booking or a pre-order.

