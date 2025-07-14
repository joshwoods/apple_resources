

- Security
-  SecKeychainItemCreatePersistentReference(\_:\_:) Deprecated

Function

# SecKeychainItemCreatePersistentReference(\_:\_:)

Creates a persistent reference for a keychain item.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainItemCreatePersistentReference(
    _ itemRef: SecKeychainItem,
    _ persistentItemRef: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`itemRef`  

A keychain item reference for the item for which you want a persistent reference.

`persistentItemRef`  

On return, a persistent reference for the keychain item. You must call the `CFRelease` function to release this object when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

Unlike normal references, a persistent reference may be stored on disk or passed between processes. You can convert a persistent reference into an ordinary keychain item reference (`SecKeychainItemRef`) by calling the SecKeychainItemCopyFromPersistentReference(_:_:) function.

