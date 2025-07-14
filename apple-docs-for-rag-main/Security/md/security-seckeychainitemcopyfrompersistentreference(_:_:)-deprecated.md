

- Security
-  SecKeychainItemCopyFromPersistentReference(\_:\_:) Deprecated

Function

# SecKeychainItemCopyFromPersistentReference(\_:\_:)

Provides a keychain item reference, given a persistent reference.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainItemCopyFromPersistentReference(
    _ persistentItemRef: CFData,
    _ itemRef: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`persistentItemRef`  

A persistent reference for a keychain item.

`itemRef`  

On return, a keychain item reference for the item for which you provided a persistent reference. You must call the `CFRelease` function to release this object when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

A persistent reference may be stored on disk or passed between processes. You use the SecKeychainItemCreatePersistentReference(_:_:) function to create a persistent reference.

