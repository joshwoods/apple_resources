

- Authentication Services
-  ASAuthorizationProviderExtensionKerberosMapping 

Class

# ASAuthorizationProviderExtensionKerberosMapping

A set of Kerberos mappings that the system login process uses.

macOS 13.0+

``` source
class ASAuthorizationProviderExtensionKerberosMapping
```

## Mentioned in 

Creating a JSON Web Encryption (JWE) login response

## Overview

This class contains a set of mappings for the sign-on token when importing the Kerberos ticket.

## Topics

### Getting the properties

var clientNameKeyName: String?

The key name of the Kerberos client name string.

var encryptionKeyTypeKeyName: String?

The key name of the Kerberos session key type number.

var messageBufferKeyName: String?

The key name of the Base 64-encoded Kerberos AS-REP string.

var realmKeyName: String?

The key name of the Kerberos realm string.

var serviceNameKeyName: String?

The key name of the Kerberos service name string.

var sessionKeyKeyName: String?

The key name of the Kerberos session key.

var ticketKeyPath: String?

The keypath in the response JSON that uses this set of mappings.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Authentication

Authentication process

Use a system-supported method to authenticate with an identity provider.

