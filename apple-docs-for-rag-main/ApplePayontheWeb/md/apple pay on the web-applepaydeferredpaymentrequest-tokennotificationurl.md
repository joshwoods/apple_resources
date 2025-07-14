

- Apple Pay on the Web
- ApplePayDeferredPaymentRequest
-  tokenNotificationURL 

Instance Property

# tokenNotificationURL

A URL to receive life-cycle notifications for the merchant-specific payment token the system issues for the request, if applicable.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
DOMString tokenNotificationURL;
```

## Discussion

If you don’t set this property, the framework doesn’t send notifications when life-cycle changes occur for the token, for example when the framework deletes the token.

## See Also

### Managing payment tokens

managementURL

A URL that links to a page on your web site where the user can manage the payment method for the deferred payment, including deleting it.

