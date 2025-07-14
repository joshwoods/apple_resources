

- Security
-  kSecAttrAccess 

Global Variable

# kSecAttrAccess

A key with a value that indicates access control list settings for the item.

macOS 10.7+

``` source
let kSecAttrAccess: CFString
```

## Discussion

The corresponding value is a SecAccess instance that describes the access control settings for this item. Create an access instance by calling the SecAccessCreate(_:_:_:) method. For more information, see Access Control Lists.

Use this attribute to set an access instance when you:

- Create a keychain item, by adding the `kSecAttrAccess` key to the dictionary you pass to SecItemAdd(_:_:).

- Modify a keychain item, by adding the `kSecAttrAccess` key to the dictionary you pass as the second parameter to SecItemUpdate(_:_:).

You can’t use this attribute to:

- Search for an item by its access instance; for example, by adding `kSecAttrAccess` to the dictionary you pass as the first parameter to SecItemUpdate(_:_:). SecItemUpdate(_:_:) and SecItemCopyMatching(_:_:) ignore this key when searching for keychain items.

- Get an item’s access instance with SecItemCopyMatching(_:_:). To get an item’s access instance, call SecKeychainItemCopyAccess(_:_:).

Important

This attribute is mutually exclusive with the kSecAttrAccessControl attribute. Also, it only applies to keychain items stored in macOS that don’t have one or both of the kSecAttrSynchronizable or kSecUseDataProtectionKeychain keys set to `true`. For information on access control for other keychain items, see Sharing access to keychain items among a collection of apps.

