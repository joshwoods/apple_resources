

- Security
-  SecKeychainFindGenericPassword(\_:\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# SecKeychainFindGenericPassword(\_:\_:\_:\_:\_:\_:\_:\_:)

Finds the first generic password based on the attributes passed.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainFindGenericPassword(
    _ keychainOrArray: CFTypeRef?,
    _ serviceNameLength: UInt32,
    _ serviceName: UnsafePointer?,
    _ accountNameLength: UInt32,
    _ accountName: UnsafePointer?,
    _ passwordLength: UnsafeMutablePointer?,
    _ passwordData: UnsafeMutablePointer?,
    _ itemRef: UnsafeMutablePointer?
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`keychainOrArray`  

A reference to an array of keychains to search, a single keychain, or `NULL` to search the user’s default keychain search list.

`serviceNameLength`  

The length of the `serviceName` character string.

`serviceName`  

A UTF-8 encoded character string representing the service name.

`accountNameLength`  

The length of the `accountName` character string.

`accountName`  

A UTF-8 encoded character string representing the account name.

`passwordLength`  

On return, the length of the buffer pointed to by `passwordData`.

`passwordData`  

On return, a pointer to a buffer that holds the password data. Pass `NULL` if you want to obtain the item object but not the password data. In this case, you must also pass `NULL` in the `passwordLength` parameter. You should use the SecKeychainItemFreeContent(_:_:) function to free the memory pointed to by this parameter.

`itemRef`  

On return, a pointer to the item object of the generic password. You are responsible for releasing your reference to this object. Pass `NULL` if you don’t want to obtain this object.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

This function finds the first generic password item that matches the attributes you provide. Most attributes are optional; you should pass only as many as you need to narrow the search sufficiently for your application’s intended use. This function optionally returns a reference to the found item.

This function decrypts the password before returning it to you. If the calling application is not in the list of trusted applications, the user is prompted before access is allowed. If the access controls for this item do not allow decryption, the function returns the `errSecAuthFailed` result code.

This function automatically calls the function SecKeychainUnlock(_:_:_:_:) to display the Unlock Keychain dialog box if the keychain is currently locked.

