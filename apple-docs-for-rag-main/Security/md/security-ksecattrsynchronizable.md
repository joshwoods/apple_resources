

- Security
-  kSecAttrSynchronizable 

Global Variable

# kSecAttrSynchronizable

A key with a value that’s a string indicating whether the item synchronizes through iCloud.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrSynchronizable: CFString
```

## Mentioned in 

Sharing access to keychain items among a collection of apps

## Discussion

The corresponding value is of type CFBoolean and indicates whether the item in question is synchronized to other devices through iCloud. To add a new synchronizable item, or to obtain synchronizable results from a query, supply this key with a value of kCFBooleanTrue. If the key is not supplied, or has a value of kCFBooleanFalse, then no synchronizable items are added or returned. Use kSecAttrSynchronizableAny to query for both synchronizable and non-synchronizable results.

A keychain item created in macOS with this attribute behaves like an iOS keychain item. For example, you share the item between apps using Access Groups instead of Access Control Lists. To create a keychain item in macOS that behaves like an iOS keychain item without making it synchronizable, use kSecUseDataProtectionKeychain instead.

The following caveats apply when you specify the kSecAttrSynchronizable key:

- You can set the kSecAttrSynchronizable key on tvOS, but tvOS doesn’t synchronize your app’s keychain items through iCloud. Items that you store on tvOS never leave the device where you create them, and items that you store on other devices don’t synchronize to tvOS devices.

- Updating or deleting items using the kSecAttrSynchronizable key affects all copies of the item, not just the one on your local device. Be sure that it makes sense to use the same password on all devices before making a password synchronizable.

- Starting in iOS 14, macOS 11, and watchOS 7, the keychain synchronizes passwords, certificates, and cryptographic keys. Earlier OS versions synchronize only passwords.

- Items stored or obtained using the kSecAttrSynchronizable key cannot specify SecAccess-based access control with kSecAttrAccess. If a password is intended to be shared between multiple applications, the kSecAttrAccessGroup key must be specified, and each application using this password must have the Keychain Access Groups Entitlement enabled, and a common access group specified.

- Items stored or obtained using the kSecAttrSynchronizable key may not also specify a kSecAttrAccessible value that is incompatible with syncing (namely, those whose names end with `ThisDeviceOnly`).

- Items stored or obtained using the kSecAttrSynchronizable key cannot be specified by reference. Use only kSecReturnAttributes and/or kSecReturnData to retrieve results.

- Do not use persistent references to synchronizable items. They cannot be moved between devices, and may not resolve if the item is modified on some other device.

- When specifying a query that uses the kSecAttrSynchronizable key, search keys are limited to the item’s class and attributes. The only search constant that may be used is kSecMatchLimit; other constants using the `kSecMatch` prefix are not supported.

