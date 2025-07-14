

- Security
-  kSecMatchLimit 

Global Variable

# kSecMatchLimit

A key whose value indicates the match limit.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecMatchLimit: CFString
```

## Mentioned in 

Searching for keychain items

Storing Keys in the Keychain

## Discussion

The corresponding value is of type CFNumber. If provided, this value specifies the maximum number of results to return or otherwise act upon. For a single item, specify kSecMatchLimitOne. To specify all matching items, specify kSecMatchLimitAll. The default behavior is function-dependent.

