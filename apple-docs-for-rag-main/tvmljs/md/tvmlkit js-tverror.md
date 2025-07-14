

- TVMLKit JS
-  TVError 

Class

# TVError

Error codes for the TVError domain.

tvOS 9.0+

``` source
interface TVError
```

## Overview

A `TVError` object encapsulates richer and more extensible error information than is possible when you use only an error code or error string. The core attributes of a `TVError` object are an error domain (represented by a string), a domain-specific error code, and a user info dictionary containing app-specific information. See User Info Dictionary Keys and Error Domains.

## Topics

### Getting Error Properties

code

The error code.

description

A string containing the description of the error.

domain

A string containing the error domain.

userInfo

The user info dictionary.

### Constants

User Info Dictionary Keys

Keys that exist in the user info dictionary.

Error Domains

The predefined error domains.

## See Also

### Errors

NSError

Information about an error condition, including a domain, a domain-specific error code, and application-specific information.

