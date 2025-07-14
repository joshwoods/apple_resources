

- Security
-  SecKeychainAttributeInfoForItemID(\_:\_:\_:) Deprecated

Function

# SecKeychainAttributeInfoForItemID(\_:\_:\_:)

Obtains tags for all possible attributes of a given item class.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainAttributeInfoForItemID(
    _ keychain: SecKeychain?,
    _ itemID: UInt32,
    _ info: UnsafeMutablePointer?>
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`keychain`  

A keychain object.

`itemID`  

The relation identifier of the item tags. An `itemID` is a `CSSM_DB_RECORDTYPE` type as defined in `cssmtype.h`.

`info`  

On return, a pointer to the keychain attribute information. Your application should call the SecKeychainFreeAttributeInfo(_:) function to release this structure when done with it.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

This call returns more attributes than are supported by the old style Keychain API and passing them into older calls yields an invalid attribute error. The recommended call to retrieve the attribute values is the SecKeychainItemCopyAttributesAndData(_:_:_:_:_:_:) function.

Note

This is a CSSM-based API. CSSM is deprecated.

For new development, where possible, you should generally use SecItemCopyMatching(_:_:) to obtain the attributes of keychain items instead, because that function is based on Core Foundation types.

