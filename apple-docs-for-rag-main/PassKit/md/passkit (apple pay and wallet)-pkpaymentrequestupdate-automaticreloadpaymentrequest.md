

- PassKit (Apple Pay and Wallet)
- PKPaymentRequestUpdate
-  automaticReloadPaymentRequest 

Instance Property

# automaticReloadPaymentRequest

The automatic reload payment request to update the payment request with.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var automaticReloadPaymentRequest: PKAutomaticReloadPaymentRequest? { get set }
```

## Discussion

The default value is nil, which indicates the automatic reload payment request needs no update.

Warning

Changing the billingAgreement along with this property causes the framework to invalidate the current payment request, close the payment sheet, and return an error in the completion handler.

You can’t use this property simultaneously with: multitoken contexts, recurring payment requests, or automatic reload payment requests.

