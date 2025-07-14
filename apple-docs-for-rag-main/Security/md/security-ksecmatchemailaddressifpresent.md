

- Security
-  kSecMatchEmailAddressIfPresent 

Global Variable

# kSecMatchEmailAddressIfPresent

A key whose value is a string to match against a certificate or identity’s email address.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecMatchEmailAddressIfPresent: CFString
```

## Discussion

The corresponding value is of type CFString and contains an RFC822 email address. If provided, returned certificates or identities are limited to those that either contain the address or do not contain any email address.

