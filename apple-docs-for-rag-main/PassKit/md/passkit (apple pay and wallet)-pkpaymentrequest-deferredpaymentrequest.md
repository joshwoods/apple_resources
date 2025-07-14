

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  deferredPaymentRequest 

Instance Property

# deferredPaymentRequest

A request to set up a deferred payment, such as a hotel booking or a pre-order.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+visionOS 1.0+

``` source
var deferredPaymentRequest: PKDeferredPaymentRequest? { get set }
```

## Discussion

Note

watchOS doesn’t support merchant-specific payment tokens.

This payment request receives a merchant-specific payment token if the payment network supports merchant-specific payment tokens.

Important

You can’t use this property simultaneously with multitoken contexts, recurring payment requests, or automatic reload payment requests. Simultaneous use of these properties results in a runtime error and cancels the payment request.

## See Also

### Requesting recurring, automatic, and deferred payments

var recurringPaymentRequest: PKRecurringPaymentRequest?

An optional request to set up a recurring payment, typically a subscription.

class PKRecurringPaymentRequest

A class that represents a request to set up a recurring payment, typically a subscription.

var automaticReloadPaymentRequest: PKAutomaticReloadPaymentRequest?

An optional request to set up an automatic reload payment, such as a store card top-up.

class PKAutomaticReloadPaymentRequest

A class that represents a request to set up an automatic reload payment, such as a store card top-up or a prepaid account.

class PKDeferredPaymentRequest

An object that represents a request to set up a deferred payment, such as a hotel booking or a pre-order.

