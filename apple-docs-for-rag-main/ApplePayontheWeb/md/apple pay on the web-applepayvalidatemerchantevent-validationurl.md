

- Apple Pay on the Web
- ApplePayValidateMerchantEvent
-  validationURL 

Instance Property

# validationURL

The URL your server must use to validate itself and obtain a merchant session object.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
readonly attribute DOMString validationURL;
```

## Mentioned in 

Providing Merchant Validation

## Discussion

This attribute is contained by the onvalidatemerchant event. Access this attribute using the event parameter, for example, `var URL = event.validationURL;`.

Pass the URL in the validationURL attribute to your server, as described in Providing Merchant Validation.

