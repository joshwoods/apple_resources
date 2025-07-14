

- Apple Pay on the Web
- ApplePayDeferredPaymentRequest
-  managementURL 

Instance Property

# managementURL

A URL that links to a page on your web site where the user can manage the payment method for the deferred payment, including deleting it.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
required DOMString managementURL;
```

## Discussion

Note

It’s a best practice to use a universal link for this URL. Using a universal link, the same link can direct a person to a page in the app (if they’ve installed the app) or to a page on the merchant’s web site. For more information on adopting universal links, see Universal links.

## See Also

### Managing payment tokens

tokenNotificationURL

A URL to receive life-cycle notifications for the merchant-specific payment token the system issues for the request, if applicable.

