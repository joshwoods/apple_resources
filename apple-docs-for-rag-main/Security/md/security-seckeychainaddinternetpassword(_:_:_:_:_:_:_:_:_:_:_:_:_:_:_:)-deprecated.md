

- Security
-  SecKeychainAddInternetPassword(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# SecKeychainAddInternetPassword(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Adds a new Internet password to a keychain.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainAddInternetPassword(
    _ keychain: SecKeychain?,
    _ serverNameLength: UInt32,
    _ serverName: UnsafePointer?,
    _ securityDomainLength: UInt32,
    _ securityDomain: UnsafePointer?,
    _ accountNameLength: UInt32,
    _ accountName: UnsafePointer?,
    _ pathLength: UInt32,
    _ path: UnsafePointer?,
    _ port: UInt16,
    _ protocol: SecProtocolType,
    _ authenticationType: SecAuthenticationType,
    _ passwordLength: UInt32,
    _ passwordData: UnsafeRawPointer,
    _ itemRef: UnsafeMutablePointer?
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`keychain`  

A reference to the keychain in which to store an Internet password. Pass `NULL` to specify the user’s default keychain.

`serverNameLength`  

The length of the `serverName` character string.

`serverName`  

A UTF-8 encoded character string representing the server name.

`securityDomainLength`  

The length of the `securityDomain` character string.

`securityDomain`  

A UTF-8 encoded character string representing the security domain. This parameter is optional. Pass NULL if the protocol does not require it.

`accountNameLength`  

The length of the `accountName` character string.

`accountName`  

A UTF-8 encoded character string representing the account name.

`pathLength`  

The length of the `path` character string.

`path`  

A UTF-8 encoded character string representing the path.

`port`  

The TCP/IP port number. If no specific port number is associated with this password, pass `0`.

`protocol`  

The protocol associated with this password. See SecProtocolType for a description of possible values.

`authenticationType`  

The authentication scheme used. See SecAuthenticationType for a description of possible values. Pass the constant `kSecAuthenticationTypeDefault`, to specify the default authentication scheme.

`passwordLength`  

The length of the `passwordData` buffer.

`passwordData`  

A pointer to a buffer containing the password data to be stored in the keychain.

`itemRef`  

On return, a pointer to a reference to the new keychain item. Pass `NULL` if you don’t want to obtain this object. You must allocate the memory for this pointer. You must call the `CFRelease` function to release this object when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes. The result code errSecNoDefaultKeychain indicates that no default keychain could be found. The result code errSecDuplicateItem indicates that you tried to add a password that already exists in the keychain. The result code errSecDataTooLarge indicates that you tried to add more data than is allowed for a structure of this type.

## Discussion

This function adds a new Internet server password to the specified keychain. Required parameters to identify the password are `serverName` and `accountName` (you cannot pass `NULL` for both parameters). In addition, some protocols may require an optional `securityDomain` when authentication is requested. This function optionally returns a reference to the newly added item.

This function sets the initial access rights for the new keychain item so that the application creating the item is given trusted access.

This function automatically calls the function SecKeychainUnlock(_:_:_:_:) to display the Unlock Keychain dialog box if the keychain is currently locked.

