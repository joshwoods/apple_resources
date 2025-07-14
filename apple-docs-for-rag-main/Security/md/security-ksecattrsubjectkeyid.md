

- Security
-  kSecAttrSubjectKeyID 

Global Variable

# kSecAttrSubjectKeyID

A key whose value indicates the item’s subject key ID.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrSubjectKeyID: CFString
```

## Discussion

The corresponding value is of type CFData and contains the subject key ID of a certificate. Items of class kSecClassCertificate have this attribute. Read only.

