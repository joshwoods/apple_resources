

- Apple Pay on the Web
- ApplePayPaymentAuthorizationResult
-  errors 

Instance Property

# errors

A list of custom errors to display on the payment sheet.

Safari Desktop 10.0+Safari Mobile 10.0+

**Unsupported OS: Safari Mobile**

``` source
sequence  errors;
```

**Unsupported OS: Safari Desktop**

``` source
sequence  errors;
```

## Discussion

List the errors on the payment sheet for the user to remedy. If there are multiple errors, list the most critical error first. For information about errors, see ApplePayError.

## See Also

### Providing authorization results

status

The status code for the authorization result.

