

- Security
- Keychain services
- Access Control Lists
-  ACL Authorization Keys 

API Collection

# ACL Authorization Keys

The operations an access control list entry applies to.

## Topics

### Constants

let kSecACLAuthorizationAny: CFString

No restrictions. This ACL entry applies to all operations available to the caller.

let kSecACLAuthorizationLogin: CFString

Use for a CSP (smart card) login.

let kSecACLAuthorizationGenKey: CFString

Generate a key.

let kSecACLAuthorizationDelete: CFString

Delete this item.

let kSecACLAuthorizationExportWrapped: CFString

Export a wrapped (that is, encrypted) key. This tag is checked on the key being exported; in addition, the `CSSM_ACL_AUTHORIZATION_ENCRYPT` tag is checked for any key used in the wrapping operation.

let kSecACLAuthorizationExportClear: CFString

Export an unencrypted key.

let kSecACLAuthorizationImportWrapped: CFString

Import an encrypted key. This tag is checked on the key being imported; in addition, the `CSSM_ACL_AUTHORIZATION_DECRYPT` tag is checked for any key used in the unwrapping operation.

let kSecACLAuthorizationImportClear: CFString

Import an unencrypted key.

let kSecACLAuthorizationSign: CFString

Digitally sign data.

let kSecACLAuthorizationEncrypt: CFString

Encrypt data.

let kSecACLAuthorizationDecrypt: CFString

Decrypt data.

let kSecACLAuthorizationMAC: CFString

Create or verify a message authentication code.

let kSecACLAuthorizationDerive: CFString

Derive a new key from another key.

let kSecACLAuthorizationKeychainCreate: CFString

Create a new keychain.

let kSecACLAuthorizationKeychainDelete: CFString

Delete a keychain.

let kSecACLAuthorizationKeychainItemRead: CFString

Read an item from a keychain.

let kSecACLAuthorizationKeychainItemInsert: CFString

Insert an item into a keychain.

let kSecACLAuthorizationKeychainItemModify: CFString

Modify an item in a keychain.

let kSecACLAuthorizationKeychainItemDelete: CFString

Delete an item from a keychain.

let kSecACLAuthorizationChangeACL: CFString

Change an access control list entry.

let kSecACLAuthorizationChangeOwner: CFString

For internal system use only. Use the `CSSM_ACL_AUTHORIZATION_CHANGE_ACL` tag for changes to owner ACL entries.

let kSecACLAuthorizationIntegrity: CFString

let kSecACLAuthorizationPartitionID: CFString

