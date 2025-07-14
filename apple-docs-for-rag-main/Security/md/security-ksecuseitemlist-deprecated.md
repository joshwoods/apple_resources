

- Security
-  kSecUseItemList Deprecated

Global Variable

# kSecUseItemList

A key whose value is an array of items to search.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0DeprecatedMac Catalyst 2.0–12.0DeprecatedmacOS 10.6+tvOS 9.0–12.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–5.0Deprecated

``` source
let kSecUseItemList: CFString
```

Deprecated

Not implemented on this platform

## Discussion

The corresponding value is of type CFArray, where the array contains either SecKeychainItem, SecKey, SecCertificate, SecIdentity, or (for persistent item references) CFData items. The items in the array must all be of the same type.

When this attribute is provided, no keychains are searched. Instead, the specified array is treated as the set of all possible items to search (or to add if the function being called is SecItemAdd(_:_:)).

