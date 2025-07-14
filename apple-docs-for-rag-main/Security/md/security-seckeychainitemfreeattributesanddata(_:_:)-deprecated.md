

- Security
-  SecKeychainItemFreeAttributesAndData(\_:\_:) Deprecated

Function

# SecKeychainItemFreeAttributesAndData(\_:\_:)

Releases the memory used by the keychain attribute list and/or the keychain data retrieved in a call to `SecKeychainItemCopyAttributesAndData`.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainItemFreeAttributesAndData(
    _ attrList: UnsafeMutablePointer?,
    _ data: UnsafeMutableRawPointer?
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`attrList`  

A pointer to the attribute list to release. Pass `NULL` if there is no attribute list to release.

`data`  

A pointer to the data buffer to release. Pass `NULL` if there is no data to release.

## Return Value

A result code. See Security Framework Result Codes.

