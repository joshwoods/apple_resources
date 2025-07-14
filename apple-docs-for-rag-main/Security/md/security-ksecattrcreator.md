

- Security
-  kSecAttrCreator 

Global Variable

# kSecAttrCreator

A key with a value that indicates the item’s creator.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrCreator: CFString
```

## Discussion

The corresponding value is of type CFNumber and represents the item’s creator. This number is the unsigned integer representation of a four-character code (for example, `'aCrt'`).

