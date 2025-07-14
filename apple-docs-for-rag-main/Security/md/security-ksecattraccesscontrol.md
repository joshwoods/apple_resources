

- Security
-  kSecAttrAccessControl 

Global Variable

# kSecAttrAccessControl

A key with a value that’s an access control instance indicating access control settings for the item.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrAccessControl: CFString
```

## Mentioned in 

Restricting keychain item accessibility

## Discussion

The corresponding value is a SecAccessControl instance, created with the SecAccessControlCreateWithFlags(_:_:_:_:) method, containing access control conditions for the item. See Restricting keychain item accessibility for more details.

Important

This attribute is mutually exclusive with the kSecAttrAccess attribute.

