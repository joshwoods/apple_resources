

- Security
-  SecKeychainItemCreateFromContent(\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# SecKeychainItemCreateFromContent(\_:\_:\_:\_:\_:\_:\_:)

Creates a new keychain item from the supplied parameters.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainItemCreateFromContent(
    _ itemClass: SecItemClass,
    _ attrList: UnsafeMutablePointer,
    _ length: UInt32,
    _ data: UnsafeRawPointer?,
    _ keychainRef: SecKeychain?,
    _ initialAccess: SecAccess?,
    _ itemRef: UnsafeMutablePointer?
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`itemClass`  

A constant identifying the class of item to create. See SecItemClass for valid constants.

`attrList`  

A pointer to the list of attributes for the item to create.

`length`  

The length of the buffer pointed to by the `data` parameter.

`data`  

A pointer to a buffer containing the data to store.

`keychainRef`  

A reference to the keychain in which to add the item. Pass `NULL` to specify the default keychain.

`initialAccess`  

An access object for this keychain item. Use the SecAccessCreate(_:_:_:) function to create an access object or the SecKeychainItemCopyAccess(_:_:) function to copy an access object from another keychain item. If you pass `NULL` for this parameter, the access defaults to the application creating the item.

`itemRef`  

On return, a pointer to a reference to the newly created keychain item. This parameter is optional. You must call the `CFRelease` function to release this object when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

Each item stored in the keychain contains data (such as a certificate), which is indexed by the item’s attributes. Use this function to create a keychain item from its attributes and data. To create keychain items that hold passwords, use the SecKeychainAddInternetPassword(_:_:_:_:_:_:_:_:_:_:_:_:_:_:_:) or SecKeychainAddGenericPassword(_:_:_:_:_:_:_:_:) functions.

A `SecKeychainItemRef` object for a certificate that is stored in a keychain can be safely cast to a `SecCertificateRef` for use with the Certificate, Key, and Trust API.

This function automatically calls the function SecKeychainUnlock(_:_:_:_:) to display the Unlock Keychain dialog box if the keychain is currently locked.

