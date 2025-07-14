

- Security
-  kSecAttrPort 

Global Variable

# kSecAttrPort

A key whose value indicates the item’s port.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrPort: CFString
```

## Discussion

The corresponding value is of type CFNumber and represents an Internet port number. Items of class kSecClassInternetPassword have this attribute.

