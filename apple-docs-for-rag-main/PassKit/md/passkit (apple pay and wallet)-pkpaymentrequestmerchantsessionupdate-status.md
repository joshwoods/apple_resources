

- PassKit (Apple Pay and Wallet)
- PKPaymentRequestMerchantSessionUpdate
-  status 

Instance Property

# status

The current authorization status for the payment.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+watchOS 7.0+

``` source
var status: PKPaymentAuthorizationStatus { get set }
```

## See Also

### Getting information for the merchant session update

var session: PKPaymentMerchantSession?

An object that validates the identity of a merchant for the payment request.

class PKPaymentMerchantSession

An object that validates the identity of a merchant for a payment request.

