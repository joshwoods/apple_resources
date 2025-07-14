

- Security
-  kSecAttrCertificateType 

Global Variable

# kSecAttrCertificateType

A key whose value indicates the item’s certificate type.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrCertificateType: CFString
```

## Discussion

The corresponding value is of type CFNumber and denotes the certificate type (see the `CSSM_CERT_TYPE` enumeration in cssmtype.h). Items of class kSecClassCertificate have this attribute. Read only.

