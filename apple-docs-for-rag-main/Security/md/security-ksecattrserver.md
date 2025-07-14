

- Security
-  kSecAttrServer 

Global Variable

# kSecAttrServer

A key whose value is a string indicating the item’s server.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrServer: CFString
```

## Mentioned in 

Adding a password to the keychain

## Discussion

The corresponding value is of type CFString and contains the server’s domain name or IP address. Items of class kSecClassInternetPassword have this attribute.

