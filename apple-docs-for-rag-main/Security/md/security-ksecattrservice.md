

- Security
-  kSecAttrService 

Global Variable

# kSecAttrService

A key whose value is a string indicating the item’s service.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrService: CFString
```

## Discussion

The corresponding value is a string of type CFString that represents the service associated with this item. Items of class kSecClassGenericPassword have this attribute.

