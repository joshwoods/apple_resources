

- Apple Pay on the Web
- ApplePayRecurringPaymentRequest
-  tokenNotificationURL 

Instance Property

# tokenNotificationURL

A URL you provide for receiving life-cycle notifications from the Apple Pay servers about the Apple Pay merchant token for the recurring payment.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
DOMString tokenNotificationURL;
```

## Discussion

The tokenNotificationURL is optional. Set this property to receive notifications for life-cycle updates to the merchant token, for example, when the card issuer or the user deletes the merchant token.

For more information about handling merchant token life-cycle notifications, see Receiving and handling merchant token notifications.

