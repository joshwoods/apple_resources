

- Security
-  SecKeychainItemSetAccess(\_:\_:) Deprecated

Function

# SecKeychainItemSetAccess(\_:\_:)

Sets the access of a given keychain item.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainItemSetAccess(
    _ itemRef: SecKeychainItem,
    _ access: SecAccess
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`itemRef`  

A keychain item.

`access`  

An access instance to replace the keychain item’s current access instance. Use the SecAccessCreate(_:_:_:) function to create a default access instance.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

Use this function to attach an access instance to a particular keychain item. Alternatively, you can use the kSecAttrAccess attribute when calling either of the SecItemAdd(_:_:) or SecItemUpdate(_:_:) methods.

