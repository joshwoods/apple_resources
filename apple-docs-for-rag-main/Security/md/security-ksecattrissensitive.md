

- Security
-  kSecAttrIsSensitive 

Global Variable

# kSecAttrIsSensitive

A key whose value indicates the item’s sensitivity.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrIsSensitive: CFString
```

## Discussion

The corresponding value is of type CFBoolean. When set to kCFBooleanTrue, the item can only be exported in an encrypted format. Items of class kSecClassKey have this attribute.

