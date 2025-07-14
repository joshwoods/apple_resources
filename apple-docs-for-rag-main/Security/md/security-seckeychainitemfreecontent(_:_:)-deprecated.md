

- Security
-  SecKeychainItemFreeContent(\_:\_:) Deprecated

Function

# SecKeychainItemFreeContent(\_:\_:)

Releases the memory used by the keychain attribute list and the keychain data retrieved in a call to the SecKeychainItemCopyContent(_:_:_:_:_:) function.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainItemFreeContent(
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

## Discussion

Because the SecKeychainFindInternetPassword(_:_:_:_:_:_:_:_:_:_:_:_:_:_:_:) and SecKeychainFindGenericPassword(_:_:_:_:_:_:_:_:) functions call the SecKeychainItemCopyContent(_:_:_:_:_:) function, you must call `SecKeychainItemFreeContent` to release the data buffers after calls to those functions as well.

Because the `SecKeychainItemCopyContent` function does not allocate buffers until they are needed, you should not call the `SecKeychainItemFreeContent` function unless data is actually returned to you.

