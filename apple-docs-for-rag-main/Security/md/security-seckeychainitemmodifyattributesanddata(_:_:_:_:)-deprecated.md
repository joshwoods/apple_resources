

- Security
-  SecKeychainItemModifyAttributesAndData(\_:\_:\_:\_:) Deprecated

Function

# SecKeychainItemModifyAttributesAndData(\_:\_:\_:\_:)

Updates an existing keychain item after changing its attributes or data.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainItemModifyAttributesAndData(
    _ itemRef: SecKeychainItem,
    _ attrList: UnsafePointer?,
    _ length: UInt32,
    _ data: UnsafeRawPointer?
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`itemRef`  

A reference to the keychain item to modify.

`attrList`  

A pointer to the list of attributes to modify and their new values. Pass `NULL` if you have no need to modify attributes.

`length`  

The length of the buffer pointed to by the `data` parameter. Pass `0` if you pass `NULL` in the `data` parameter.

`data`  

A pointer to a buffer containing the data to store. Pass `NULL` if you do not need to modify the data.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

The keychain item is written to the keychain’s permanent data store. If the keychain item has not previously been added to a keychain, a call to this function does nothing and returns `noErr`.

Note

For new development, where possible, you should generally use SecItemUpdate(_:_:) to obtain attributes of keychain items instead, because that function is based on Core Foundation types.

Note that when you use this function to modify a keychain item, Keychain Services updates the modification date of the item. Therefore, you cannot use this function to modify the modification date, as the value you specify will be overwritten with the current time. If you want to change the modification date to something other than the current time, use a CSSM function to do so.

You should pair the SecKeychainItemCopyAttributesAndData(_:_:_:_:_:_:) function with the `SecKeychainItemModifyAttributesAndData` function, as these functions handle more attributes than are support by the old Keychain Manager and passing them into older calls yields an invalid attribute error. Use the functions SecKeychainItemModifyContent(_:_:_:_:) and SecKeychainItemCopyContent(_:_:_:_:_:) when dealing with older Keychain Manager functions.

