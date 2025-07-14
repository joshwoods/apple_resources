

- Apple Pay on the Web
- ApplePaySession
-  ApplePaySession 

Initializer

# ApplePaySession

The entry point for Apple Pay on the web.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
new ApplePaySession();
```

## Parameters 

`version`  

The Apple Pay version number your website supports. See Apple Pay on the web version history for version information.

`paymentRequest`  

An ApplePayPaymentRequest object that contains the information to be displayed on the Apple Pay payment sheet.

## Mentioned in 

Apple Pay on the Web Version 12 Release Notes

Creating an Apple Pay Session

## Discussion

Creating an `ApplePaySession` object throws a JavaScript exception if any of the following occur:

- Any Apple Pay JS API is called from an insecure page.

- You pass an invalid payment request. Payment requests are invalid if they contain missing, unknown, or invalid properties, or if the total is zero or less.

- You attempt to create ApplePaySession outside of a gesture handler.

Check supportsVersion before using any Apple Pay JS API that depends on Safari to support a particular version number.

## See Also

### Related Documentation

begin

Begins the merchant validation process.

supportsVersion

Detects whether a web browser supports a particular Apple Pay version.

