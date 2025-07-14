

- Security
-  kSecMatchSearchList 

Global Variable

# kSecMatchSearchList

A key whose value indicates a list of items to search.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecMatchSearchList: CFString
```

## Discussion

The value is a CFArray of SecKeychain items. If provided, the search will be limited to the keychain items contained in this list.

