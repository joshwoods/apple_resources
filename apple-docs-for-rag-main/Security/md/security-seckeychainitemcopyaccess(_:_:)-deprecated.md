

- Security
-  SecKeychainItemCopyAccess(\_:\_:) Deprecated

Function

# SecKeychainItemCopyAccess(\_:\_:)

Retrieves the access of a given keychain item.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainItemCopyAccess(
    _ itemRef: SecKeychainItem,
    _ access: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`itemRef`  

A keychain item.

`access`  

On return, points to the keychain item’s access instance. Call the CFRelease method to release this access instance when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

Use this method to retrieve the access instance from a keychain item. Alternatively, you can look for the kSecAttrAccess attribute among the keychain item’s attributes when you call the SecItemCopyMatching(_:_:) method.

