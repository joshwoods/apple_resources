

- PassKit (Apple Pay and Wallet)
- PKAutomaticReloadPaymentRequest
-  tokenNotificationURL 

Instance Property

# tokenNotificationURL

A URL you provide to receive life-cycle notifications from the Apple Pay servers about the Apple Pay merchant token for the automatic reload payment.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var tokenNotificationURL: URL? { get set }
```

## Discussion

The tokenNotificationURL is optional. Set this property to receive notifications for life-cycle updates to the merchant token, for example, when the card issuer or the user deletes the token.

For more information about handling merchant token life-cycle notifications, see Receiving and handling merchant token notifications.

## See Also

### Managing payment tokens

var managementURL: URL

A URL to a web page where the user can manage and delete the payment method for the automatic reload payment.

