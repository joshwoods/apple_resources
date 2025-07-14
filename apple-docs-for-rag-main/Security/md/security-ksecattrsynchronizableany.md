

- Security
-  kSecAttrSynchronizableAny 

Global Variable

# kSecAttrSynchronizableAny

Specifies that both synchronizable and non-synchronizable results should be returned from a query.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrSynchronizableAny: CFString
```

## Discussion

This may be used as a value for the kSecAttrSynchronizable dictionary key (in place of `kCFBooleanTrue` or `kCFBooleanFalse`) in a call to SecItemCopyMatching(_:_:), SecItemUpdate(_:_:), or SecItemDelete(_:).

