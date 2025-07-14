

- Security
-  kSecAttrSerialNumber 

Global Variable

# kSecAttrSerialNumber

A key whose value indicates the item’s serial number.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrSerialNumber: CFString
```

## Discussion

The corresponding value is of type CFData and contains the serial number data of a certificate. Items of class kSecClassCertificate have this attribute. Read only.

