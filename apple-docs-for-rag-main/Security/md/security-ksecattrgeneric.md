

- Security
-  kSecAttrGeneric 

Global Variable

# kSecAttrGeneric

A key whose value indicates the item’s user-defined attributes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrGeneric: CFString
```

## Discussion

The corresponding value is of type CFData and contains a user-defined attribute. Items of class kSecClassGenericPassword have this attribute.

