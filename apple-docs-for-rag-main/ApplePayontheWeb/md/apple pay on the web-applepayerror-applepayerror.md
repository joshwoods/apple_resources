

- Apple Pay on the Web
- ApplePayError
-  ApplePayError 

Initializer

# ApplePayError

Creates an Apple Pay error object.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
new errorCode(
 ApplePayErrorCode errorCode,
 optional ApplePayErrorContactField contactField,
 optional DOMString message
);
```

## Discussion

ApplePayError objects are created using a constructor, as follows:

```
```

The contact field, ApplePayErrorContactField, and message parameters are optional. Use them to provide more detailed information that can help users resolve problems on the payment sheet. Some error codes do not require a contact field parameter. See ApplePayErrorCode for more information.

