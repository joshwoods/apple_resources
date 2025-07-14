

- PassKit (Apple Pay and Wallet)
- PKAutomaticReloadPaymentRequest
-  paymentDescription 

Instance Property

# paymentDescription

A description that you provide of the automatic reload payment and that Apple Pay displays to the user in the payment sheet.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var paymentDescription: String { get set }
```

## Discussion

Provide a display name for the automatic reload, for example, “Gift Card Reload”.

## See Also

### Describing an automatic reload payment

var billingAgreement: String?

A localized billing agreement that the payment sheet displays to the user before the user authorizes the payment.

