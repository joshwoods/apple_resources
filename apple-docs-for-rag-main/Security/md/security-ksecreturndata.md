

- Security
-  kSecReturnData 

Global Variable

# kSecReturnData

A key whose value is a Boolean that indicates whether or not to return item data.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecReturnData: CFString
```

## Mentioned in 

Searching for keychain items

## Discussion

The corresponding value is of type CFBoolean. A value of kCFBooleanTrue indicates that the function needs to return the item’s data as a CFData object.

For keys and password items, data is secret (encrypted) and might require the user to enter a password for access. For key items, the resulting data has the same format as the return value of the function SecKeyCopyExternalRepresentation(_:_:). However, the key data might not be extractable (for example, if it’s protected by the Secure Enclave), so prefer to use SecKeyCopyExternalRepresentation(_:_:) for keys and check the `error` parameter if it returns `nil`.

