

- PassKit (Apple Pay and Wallet)
- PKDeferredPaymentRequest
-  tokenNotificationURL 

Instance Property

# tokenNotificationURL

A URL to receive life-cycle notifications for the merchant-specific payment token the system issues for the request, if applicable.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+visionOS 1.0+

``` source
var tokenNotificationURL: URL? { get set }
```

## Discussion

If you don’t set this property, the framework doesn’t send notifications when life-cycle changes occur for the token, for example when the framework deletes the token.

## See Also

### Managing payment tokens

var managementURL: URL

A URL that links to a page on your web site where the user can manage the payment method for the deferred payment, including deleting it.

