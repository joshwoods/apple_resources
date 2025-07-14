

- Security
-  SecKeychainItemCreateCopy(\_:\_:\_:\_:) Deprecated

Function

# SecKeychainItemCreateCopy(\_:\_:\_:\_:)

Copies a keychain item from one keychain to another.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainItemCreateCopy(
    _ itemRef: SecKeychainItem,
    _ destKeychainRef: SecKeychain?,
    _ initialAccess: SecAccess?,
    _ itemCopy: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`itemRef`  

A reference to the keychain item to copy.

`destKeychainRef`  

A reference to the keychain in which to insert the copied keychain item. Pass `NULL` to specify the default keychain.

`initialAccess`  

The initial access for the copied keychain item. Use the SecAccessCreate(_:_:_:) function to create an access object or the SecKeychainItemCopyAccess(_:_:) function to copy an access object from another keychain item. If you pass `NULL` for this parameter, the access defaults to the application creating the item.

`itemCopy`  

On return, a pointer to a copy of the keychain item referenced by the `itemRef` parameter. You must call the `CFRelease` function to release this object when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes.

