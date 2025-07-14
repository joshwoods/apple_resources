

- Security
-  kSecAttrApplicationLabel 

Global Variable

# kSecAttrApplicationLabel

A key whose value indicates the item’s application label.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrApplicationLabel: CFString
```

## Discussion

The corresponding value is of type doc://com.apple.documentation/documentation/corefoundation/cfdata-rv9 and contains a label for this item. This attribute is different from the kSecAttrLabel attribute, which is intended to be human-readable. Instead, this attribute is used to look up a key programmatically; in particular, for keys of class kSecAttrKeyClassPublic and kSecAttrKeyClassPrivate, the value of this attribute is the hash of the public key.

