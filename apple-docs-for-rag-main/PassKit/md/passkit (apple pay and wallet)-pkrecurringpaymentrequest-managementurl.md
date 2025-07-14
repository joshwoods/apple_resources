

- PassKit (Apple Pay and Wallet)
- PKRecurringPaymentRequest
-  managementURL 

Instance Property

# managementURL

A URL to a web page where the user can update or delete the payment method for the recurring payment.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var managementURL: URL { get set }
```

## Discussion

When users remove a payment method, the system deletes the associated Apple Pay merchant token.

Note

It’s a best practice to use a universal link for this URL. Using a universal link, the same link can direct a person to a page in the app (if they’ve installed the app) or to a page on the merchant’s web site. For more information on adopting universal links, see Universal links.

## See Also

### Managing payment tokens

var tokenNotificationURL: URL?

A URL you provide to receive life-cycle notifications from the Apple Pay servers about the Apple Pay merchant token for the recurring payment.

