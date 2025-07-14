

- ARKit
-  ar_error_get_error_code 

Function

# ar_error_get_error_code

Gets the error code associated with an error.

visionOS 1.0+

``` source
extern ar_error_code_t ar_error_get_error_code(ar_error_t error);
```

## See Also

### Errors

ar_error_t

An error reported by ARKit.

ar_error_code_t

Codes that identify errors in ARKit.

ar_error_domain

A string that indicates the error domain in Core Foundation.

ar_error_copy_cf_error

Copies a reference to a Core Foundation error object that represents the specified ARKit error.

