

- Security
-  SecCertificate 

Class

# SecCertificate

An abstract Core Foundation-type object representing an X.509 certificate.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class SecCertificate
```

## Mentioned in 

Storing a DER-Encoded X.509 Certificate

Getting a Certificate

Storing an Identity in the Keychain

## Overview

A SecCertificate object for a certificate that is stored in a keychain can be safely cast to a SecKeychainItem for manipulation as a keychain item. On the other hand, if the SecCertificate is not stored in a keychain, casting the object to a SecKeychainItem and passing it to Keychain Services functions returns errors.

## Relationships

### Conforms To

- Equatable
- Hashable

