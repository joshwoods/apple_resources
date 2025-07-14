

- Security
-  kSecAttrApplicationTag 

Global Variable

# kSecAttrApplicationTag

A key whose value indicates the item’s private tag.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrApplicationTag: CFString
```

## Mentioned in 

Generating New Cryptographic Keys

## Discussion

The corresponding value is of type CFData and contains private tag data.

On key creation, if not explicitly specified, this attribute defaults to `NULL`.

