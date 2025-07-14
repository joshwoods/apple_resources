

- PassKit (Apple Pay and Wallet)
- PKDeferredPaymentRequest
-  managementURL 

Instance Property

# managementURL

A URL that links to a page on your web site where the user can manage the payment method for the deferred payment, including deleting it.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+visionOS 1.0+

``` source
var managementURL: URL { get set }
```

## Discussion

Note

It’s a best practice to use a universal link for this URL. Using a universal link, the same link can direct a person to a page in the app (if they’ve installed the app) or to a page on the merchant’s web site. For more information on adopting universal links, see Universal links.

## See Also

### Managing payment tokens

var tokenNotificationURL: URL?

A URL to receive life-cycle notifications for the merchant-specific payment token the system issues for the request, if applicable.

