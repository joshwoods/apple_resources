

- Security
-  kSecAttrCertificateEncoding 

Global Variable

# kSecAttrCertificateEncoding

A key whose value indicates the item’s certificate encoding.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrCertificateEncoding: CFString
```

## Discussion

The corresponding value is of type CFNumber and denotes the certificate encoding (see the `CSSM_CERT_ENCODING` enumeration in cssmtype.h). Items of class kSecClassCertificate have this attribute. Read only.

