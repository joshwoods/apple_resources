

- Apple Pay on the Web
- ApplePaySession
-  onvalidatemerchant 

Instance Property

# onvalidatemerchant

An event handler the system calls when it displays the payment sheet.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
attribute EventHandler onvalidatemerchant;
```

## Mentioned in 

Providing Merchant Validation

Requesting an Apple Pay payment session

## Discussion

Use this attribute to request and return a merchant session. You must set this attribute to the following function:

```
session.onvalidatemerchant = function(event) {}
```

where `event` is an ApplePayValidateMerchantEvent object.

The process to complete the merchant validation is as follows:

1.  Your onvalidatemerchant function calls your server, and passes it the static hostname `apple-pay-gateway.apple.com` as the validation URL. In the China region, use `cn-apple-pay-gateway.apple.com`.

2.  Your server uses the validation URL to request a session from the Apple Pay server, as described in Requesting an Apple Pay payment session.

3.  In response, your server receives an opaque merchant session object, `MerchantSession`.

4.  You pass the merchant session object to the completion method, completeMerchantValidation.

The system enables the payment sheet.

Note

Previous merchant validation instructions stated that your onvalidatemerchant function must call your server and pass it the URL from the event’s validationURL attribute. Apple Pay continues to support this flow for existing implementations.

## See Also

### Related Documentation

Providing Merchant Validation

Validate your merchant identity and receive a session object for each payment request.

### Getting merchant validation

begin

Begins the merchant validation process.

completeMerchantValidation

Completes the validation for a merchant session.

ApplePayValidateMerchantEvent

An event object that contains the validation URL.

