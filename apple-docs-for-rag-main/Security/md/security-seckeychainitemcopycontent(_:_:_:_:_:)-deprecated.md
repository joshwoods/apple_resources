

- Security
-  SecKeychainItemCopyContent(\_:\_:\_:\_:\_:) Deprecated

Function

# SecKeychainItemCopyContent(\_:\_:\_:\_:\_:)

Copies the data and attributes stored in the given keychain item.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainItemCopyContent(
    _ itemRef: SecKeychainItem,
    _ itemClass: UnsafeMutablePointer?,
    _ attrList: UnsafeMutablePointer?,
    _ length: UnsafeMutablePointer?,
    _ outData: UnsafeMutablePointer?
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`itemRef`  

A reference to the keychain item to modify.

`itemClass`  

On return, points to the item’s class. Pass `NULL` if it is not required. See SecItemClass for valid constants.

`attrList`  

On entry, the list of attributes to get in this item; on return the attributes are filled in. Pass `NULL` if you don’t need to retrieve any attributes. You must call SecKeychainItemFreeContent(_:_:) when you no longer need the attributes and data.

`length`  

On return, the length of the buffer pointed to by the `outData` parameter.

`outData`  

On return, a pointer to a buffer containing the data in this item. Pass `NULL` if you don’t need this data. You must call SecKeychainItemFreeContent(_:_:) when you no longer need the attributes and data.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

This function returns the data and attributes of a specific keychain item.

Note

For new development, where possible, you should generally use SecItemCopyMatching(_:_:) to obtain the data and attributes of keychain items instead, because that function is based on Core Foundation types.

You can use the SecKeychainSearchCopyNext function to search for a keychain item if you don’t already have the item’s reference object. To find and obtain data from a password keychain item, use the SecKeychainFindInternetPassword(_:_:_:_:_:_:_:_:_:_:_:_:_:_:_:) or SecKeychainFindGenericPassword(_:_:_:_:_:_:_:_:) function.

You should pair the SecKeychainItemModifyContent(_:_:_:_:) function with the `SecKeychainItemCopyContent` function when dealing with older Keychain Manager functions. The SecKeychainItemCopyAttributesAndData(_:_:_:_:_:_:) and SecKeychainItemModifyAttributesAndData(_:_:_:_:) functions handle more attributes than are supported by the old Keychain Manager; however, passing them into older calls yields an invalid attribute error.

If the keychain item data is encrypted, this function decrypts the data before returning it to you. If the calling application is not in the list of trusted applications, the user is prompted before access is allowed. If the access controls for this item do not allow decryption, the function returns the `errSecAuthFailed` result code.

