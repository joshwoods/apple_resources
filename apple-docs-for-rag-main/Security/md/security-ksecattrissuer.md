

- Security
-  kSecAttrIssuer 

Global Variable

# kSecAttrIssuer

A key whose value indicates the item’s issuer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrIssuer: CFString
```

## Discussion

The corresponding value is of type CFData and contains the X.500 issuer name of a certificate. Items of class kSecClassCertificate have this attribute. Read only.

