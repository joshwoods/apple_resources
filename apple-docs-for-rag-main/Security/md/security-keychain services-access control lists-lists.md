

- Security
- Keychain services
-  Access Control Lists 

API Collection

# Access Control Lists

Control which apps have access to keychain items in macOS.

## Overview

In macOS, for items not stored on the iCloud keychain, each protected keychain item—like a password or private key—has an associated access instance that contains an access control list (ACL). The entries in this list in turn each contain an array of operations and an array of apps trusted to carry out those operations with the item. The collection of ACL entries govern the accessibility of the corresponding keychain item.

When an app attempts to access a keychain item for a particular purpose—like using a private key to sign a document—the system looks for an entry in the item’s ACL containing the operation. If there’s no entry that lists the operation, then the system denies access and it’s up to the calling app to try something else or to notify the user.

If there is an entry that lists the operation, the system checks whether the calling app is among the entry’s trusted apps. If so, the system grants access. Otherwise, the system prompts the user for confirmation. The user may choose to Deny, Allow, or Always Allow the access. In the latter case, the system adds the app to the list of trusted apps for that entry, enabling the app to gain access in the future without prompting the user again.

Important

ACLs are not available in iOS or in macOS apps that use the iCloud keychain. For keychain item sharing in those environments, use access groups instead. See Sharing access to keychain items among a collection of apps.

## Topics

### Access Creation

func SecAccessCreate(CFString, CFArray?, UnsafeMutablePointer&lt;SecAccess?>) -> OSStatus

Creates a new access instance associated with a given protected keychain item.

Deprecated

func SecAccessCreateWithOwnerAndACL(uid_t, gid_t, SecAccessOwnerType, CFArray?, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> SecAccess?

Creates a new access instance using the owner and ACL entries you provide.

Deprecated

typealias SecAccessOwnerType

A type for flags that enable you to configure ACL ownership.

SecAccessOwnerType Values

Flags that enable you to configure ACL ownership.

class SecAccess

An opaque type that identifies a keychain item’s access information.

func SecAccessGetTypeID() -> CFTypeID

Returns the unique identifier of the opaque type to which an access instance belongs.

Deprecated

### Access Query

func SecAccessCopyACLList(SecAccess, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Retrieves all the ACL entries of a given access instance.

Deprecated

func SecAccessCopyMatchingACLList(SecAccess, CFTypeRef) -> CFArray?

Retrieves selected ACL entries from a given access instance.

Deprecated

func SecAccessCopyOwnerAndACL(SecAccess, UnsafeMutablePointer&lt;uid_t>?, UnsafeMutablePointer&lt;gid_t>?, UnsafeMutablePointer&lt;SecAccessOwnerType>?, UnsafeMutablePointer&lt;CFArray?>?) -> OSStatus

Retrieves the owner and the ACL entries of a given access instance.

Deprecated

### Access Control List Entries

func SecACLCreateWithSimpleContents(SecAccess, CFArray?, CFString, SecKeychainPromptSelector, UnsafeMutablePointer&lt;SecACL?>) -> OSStatus

Creates a new ACL entry with the given characteristics, and adds it to an access instance.

Deprecated

func SecACLRemove(SecACL) -> OSStatus

Removes the specified ACL entry from the access instance that contains it.

Deprecated

ACL Authorization Keys

The operations an access control list entry applies to.

struct SecKeychainPromptSelector

Bits that define when a keychain should require a passphrase.

class SecACL

An opaque type that represents information about an ACL entry.

func SecACLGetTypeID() -> CFTypeID

Returns the unique identifier of the opaque type to which an ACL entry belongs.

Deprecated

### Access Control List Configuration

func SecACLCopyContents(SecACL, UnsafeMutablePointer&lt;CFArray?>, UnsafeMutablePointer&lt;CFString?>, UnsafeMutablePointer&lt;SecKeychainPromptSelector>) -> OSStatus

Returns the application list, description, and prompt selector for a given ACL entry.

Deprecated

func SecACLSetContents(SecACL, CFArray?, CFString, SecKeychainPromptSelector) -> OSStatus

Sets the application list, description, and prompt selector for a given ACL entry.

Deprecated

func SecACLCopyAuthorizations(SecACL) -> CFArray

Retrieves the authorization tags of a given ACL entry.

Deprecated

func SecACLUpdateAuthorizations(SecACL, CFArray) -> OSStatus

Sets the authorization tags for a given ACL.

Deprecated

### Trusted Applications

func SecTrustedApplicationCreateFromPath(UnsafePointer&lt;CChar>?, UnsafeMutablePointer&lt;SecTrustedApplication?>) -> OSStatus

Creates a trusted app instance based on the app at the given path in the file system.

Deprecated

func SecTrustedApplicationCopyData(SecTrustedApplication, UnsafeMutablePointer&lt;CFData?>) -> OSStatus

Retrieves the data of a trusted app instance.

Deprecated

func SecTrustedApplicationSetData(SecTrustedApplication, CFData) -> OSStatus

Sets the data of a given trusted app instance.

Deprecated

class SecTrustedApplication

An opaque type that contains information about a trusted app.

func SecTrustedApplicationGetTypeID() -> CFTypeID

Returns the unique identifier of the opaque type to which a trusted app instance belongs.

Deprecated

### Keychain Item Access

func SecKeychainItemSetAccess(SecKeychainItem, SecAccess) -> OSStatus

Sets the access of a given keychain item.

Deprecated

func SecKeychainItemCopyAccess(SecKeychainItem, UnsafeMutablePointer&lt;SecAccess?>) -> OSStatus

Retrieves the access of a given keychain item.

Deprecated

