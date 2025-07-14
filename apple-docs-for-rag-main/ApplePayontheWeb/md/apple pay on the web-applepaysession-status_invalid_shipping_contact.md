

- Apple Pay on the Web
- ApplePaySession
-  STATUS_INVALID_SHIPPING_CONTACT 

# STATUS_INVALID_SHIPPING_CONTACT

The shipping contact information is invalid.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
const unsigned short STATUS_INVALID_SHIPPING_CONTACT;
```

## Discussion

Use this status code only for Apple Pay API version 1 or 2 style calls. For version 3, use an ApplePayError with a status of STATUS_FAILURE and error code instead.

The payment sheet remains open and shows the email address and/or phone number highlighted in red.

## See Also

### Related Documentation

supportsVersion

Detects whether a web browser supports a particular Apple Pay version.

### Status code constants

STATUS_FAILURE

The requested action failed.

STATUS_INVALID_BILLING_POSTAL_ADDRESS

The billing address is invalid.

STATUS_INVALID_SHIPPING_POSTAL_ADDRESS

The shipping address is invalid.

STATUS_PIN_INCORRECT

The PIN information is not valid.

STATUS_PIN_LOCKOUT

The maximum number of tries for a PIN has been reached and the user has been locked out.

STATUS_PIN_REQUIRED

The required PIN information was not provided.

STATUS_SUCCESS

The requested action succeeded.

