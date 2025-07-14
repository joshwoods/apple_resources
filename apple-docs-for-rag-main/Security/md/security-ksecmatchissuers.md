

- Security
-  kSecMatchIssuers 

Global Variable

# kSecMatchIssuers

A key whose value is a string to match against a certificate or identity’s issuers.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecMatchIssuers: CFString
```

## Discussion

The corresponding value is of type CFArray, where the array consists of X.500 names of type CFData. If provided, returned certificates or identities are limited to those whose certificate chain contains one of the issuers provided in this list.

