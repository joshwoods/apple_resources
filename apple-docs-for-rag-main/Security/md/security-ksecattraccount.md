

- Security
-  kSecAttrAccount 

Global Variable

# kSecAttrAccount

A key whose value is a string indicating the item’s account name.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrAccount: CFString
```

## Mentioned in 

Searching for keychain items

Updating and deleting keychain items

## Discussion

The corresponding value is of type CFString and contains an account name. Items of class kSecClassGenericPassword and kSecClassInternetPassword have this attribute.

