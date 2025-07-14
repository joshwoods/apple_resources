

- Security
-  kSecValueData 

Global Variable

# kSecValueData

A key whose value is the item’s data.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecValueData: CFString
```

## Mentioned in 

Searching for keychain items

Updating and deleting keychain items

## Discussion

The corresponding value is of type CFData.  For keys and password items, the data is secret (encrypted) and may require the user to enter a password for access.

