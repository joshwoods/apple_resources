

- Security
-  SecKeychainItemCopyKeychain(\_:\_:) Deprecated

Function

# SecKeychainItemCopyKeychain(\_:\_:)

Returns the keychain object of a given keychain item.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainItemCopyKeychain(
    _ itemRef: SecKeychainItem,
    _ keychainRef: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`itemRef`  

A keychain item object.

`keychainRef`  

On return, a pointer to a keychain object referencing the given keychain item. You must call the `CFRelease` function to release this object when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes.

