

- TVMLKit JS
-  NSError 

Class

# NSError

Information about an error condition, including a domain, a domain-specific error code, and application-specific information.

tvOS 11.0+

``` source
interface NSError
```

## Topics

### Getting Error Properties

code

The error code.

domain

A string containing the error domain.

userInfo

The user info dictionary.

underlyingError

The error that was encountered in an underlying implementation and caused the error that the receiver represents to occur.

### Getting a Localized Error Description

description

A string containing the localized description of the error.

failureReason

A string containing the localized explanation of the reason for the error.

recoverySuggestion

A string containing the localized recovery suggestion for the error.

## See Also

### Errors

TVError

Error codes for the TVError domain.

