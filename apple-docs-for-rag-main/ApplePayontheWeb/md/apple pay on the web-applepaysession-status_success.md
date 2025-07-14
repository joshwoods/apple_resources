

- Apple Pay on the Web
- ApplePaySession
-  STATUS_SUCCESS 

# STATUS_SUCCESS

The requested action succeeded.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
const unsigned short STATUS_SUCCESS;
```

## Discussion

When you call completePayment with STATUS_SUCCESS, the payment sheet shows that the transaction was successful, and the sheet is dismissed . For all other methods, the payment sheet remains open.

## See Also

### Status code constants

STATUS_FAILURE

The requested action failed.

STATUS_INVALID_BILLING_POSTAL_ADDRESS

The billing address is invalid.

STATUS_INVALID_SHIPPING_CONTACT

The shipping contact information is invalid.

STATUS_INVALID_SHIPPING_POSTAL_ADDRESS

The shipping address is invalid.

STATUS_PIN_INCORRECT

The PIN information is not valid.

STATUS_PIN_LOCKOUT

The maximum number of tries for a PIN has been reached and the user has been locked out.

STATUS_PIN_REQUIRED

The required PIN information was not provided.

