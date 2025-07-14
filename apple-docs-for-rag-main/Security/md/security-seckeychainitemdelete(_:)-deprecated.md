

- Security
-  SecKeychainItemDelete(\_:) Deprecated

Function

# SecKeychainItemDelete(\_:)

Deletes a keychain item from the default keychain’s permanent data store.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainItemDelete(_ itemRef: SecKeychainItem) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`itemRef`  

A keychain item object of the item to delete. You must call the `CFRelease` function to release this object when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

If the keychain item has not previously been added to the keychain, this function does nothing and returns `noErr`.

Do not delete a keychain item and recreate it in order to modify it; instead, use the SecKeychainItemModifyContent(_:_:_:_:) or SecKeychainItemModifyAttributesAndData(_:_:_:_:) function to modify an existing keychain item. When you delete a keychain item, you lose any access controls and trust settings added by the user or by other applications.

