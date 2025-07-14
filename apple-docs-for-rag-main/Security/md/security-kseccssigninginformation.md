

- Security
-  kSecCSSigningInformation 

Global Variable

# kSecCSSigningInformation

Cryptographic signing information.

Mac Catalyst 13.0+macOS 10.0+

``` source
var kSecCSSigningInformation: UInt32 { get }
```

## Discussion

The certificate chain and Cryptographic Message Syntax (CMS) data (if any). For ad-hoc signed code, there are no certificates and the CMS data is empty.

