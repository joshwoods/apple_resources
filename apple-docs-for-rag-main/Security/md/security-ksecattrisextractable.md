

- Security
-  kSecAttrIsExtractable 

Global Variable

# kSecAttrIsExtractable

A key whose value indicates the item’s extractability.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrIsExtractable: CFString
```

## Discussion

The corresponding value is of type CFBoolean and indicates whether the item can be exported from its keychain. Items of class kSecClassKey have this attribute.

