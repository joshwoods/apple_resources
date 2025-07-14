

- Security
-  kSecAttrLabel 

Global Variable

# kSecAttrLabel

A key with a value that’s a string indicating the item’s label.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrLabel: CFString
```

## Mentioned in 

Storing a Certificate in the Keychain

Adding a password to the keychain

## Discussion

The corresponding value is of type CFString and contains the user-visible label for this item.

On key creation, if not explicitly specified, this attribute defaults to `NULL`.

