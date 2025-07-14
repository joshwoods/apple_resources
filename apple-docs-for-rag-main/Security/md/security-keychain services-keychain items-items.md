

- Security
- Keychain services
-  Keychain items 

API Collection

# Keychain items

Embed confidential information in items that you store in a keychain.

## Overview

When you want to store a secret such as a password or cryptographic key, you package it as a keychain item. Along with the data itself, you provide a set of publicly visible attributes both to control the item’s accessibility and to make it searchable. As shown in Figure 1, keychain services handles data encryption and storage (including data attributes) in a keychain, which is an encrypted database stored on disk. Later, authorized processes use keychain services to find the item and decrypt its data.

## Topics

### Essentials

Using the keychain to manage user secrets

Relieve the user of remembering small secrets by storing them in the keychain.

TN3137: On Mac keychain APIs and implementations

Learn how the keychain on macOS differs from other Apple platforms.

class SecKeychainItem

An opaque type that represents a keychain item.

func SecKeychainItemGetTypeID() -> CFTypeID

Returns the unique identifier of the opaque type to which a keychain item object belongs.

Deprecated

### Adding keychain items

Adding a password to the keychain

Add network credentials to the keychain on behalf of the user.

func SecItemAdd(CFDictionary, UnsafeMutablePointer&lt;CFTypeRef?>?) -> OSStatus

Adds one or more items to a keychain.

Item class keys and values

Specify the class of a keychain item.

Item attribute keys and values

Specify the attributes of keychain items.

### Keychain item search

Searching for keychain items

Find keychain items based on search criteria that you specify.

func SecItemCopyMatching(CFDictionary, UnsafeMutablePointer&lt;CFTypeRef?>?) -> OSStatus

Returns one or more keychain items that match a search query, or copies attributes of specific keychain items.

Search attribute keys and values

Filter a keychain item search.

Item return result keys

Specify how you want returned keychain item data formatted.

### Keychain item modification

Updating and deleting keychain items

Modify items in the keychain when the user’s data changes.

func SecItemUpdate(CFDictionary, CFDictionary) -> OSStatus

Modifies items that match a search query.

func SecItemDelete(CFDictionary) -> OSStatus

Deletes items that match a search query.

### Keychain item access

Sharing access to keychain items among a collection of apps

Enable apps to share keychain items with each other by adding the apps to an access group.

Keychain Access Groups Entitlement

The identifiers for the keychain groups that the app may share items with.

Restricting keychain item accessibility

Set the conditions under which an app can access a keychain item such as a password.

func SecAccessControlCreateWithFlags(CFAllocator?, CFTypeRef, SecAccessControlCreateFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> SecAccessControl?

Creates a new access control object with the specified protection type and flags.

struct SecAccessControlCreateFlags

Access control constants that dictate how a keychain item may be used.

class SecAccessControl

An opaque type that contains information about how a keychain item may be used.

func SecAccessControlGetTypeID() -> CFTypeID

Returns the unique identifier of the opaque type to which a keychain item access control object belongs.

### Import and export

func SecItemImport(CFData, CFString?, UnsafeMutablePointer&lt;SecExternalFormat>?, UnsafeMutablePointer&lt;SecExternalItemType>?, SecItemImportExportFlags, UnsafePointer&lt;SecItemImportExportKeyParameters>?, SecKeychain?, UnsafeMutablePointer&lt;CFArray?>?) -> OSStatus

Imports one or more certificates, keys, or identities and optionally adds them to a keychain.

func SecItemExport(CFTypeRef, SecExternalFormat, SecItemImportExportFlags, UnsafePointer&lt;SecItemImportExportKeyParameters>?, UnsafeMutablePointer&lt;CFData?>) -> OSStatus

Exports one or more certificates, keys, or identities.

enum SecExternalFormat

The external format of a keychain item.

enum SecExternalItemType

The import item type.

struct SecItemImportExportFlags

The import and export function flags.

struct SecItemImportExportKeyParameters

The import/export parameter structure.

struct SecKeyImportExportFlags

The import/export parameter structure flags.

var SEC_KEY_IMPORT_EXPORT_PARAMS_VERSION: Int32

The import/export parameter structure version.

struct SecKeyImportExportParameters

The legacy import/export parameter structure.

Deprecated

### Legacy keychain item creation

Use the functions in Adding keychain items instead.

func SecKeychainItemCreateFromContent(SecItemClass, UnsafeMutablePointer&lt;SecKeychainAttributeList>, UInt32, UnsafeRawPointer?, SecKeychain?, SecAccess?, UnsafeMutablePointer&lt;SecKeychainItem?>?) -> OSStatus

Creates a new keychain item from the supplied parameters.

Deprecated

func SecKeychainItemCreateCopy(SecKeychainItem, SecKeychain?, SecAccess?, UnsafeMutablePointer&lt;SecKeychainItem?>) -> OSStatus

Copies a keychain item from one keychain to another.

Deprecated

func SecKeychainItemCreatePersistentReference(SecKeychainItem, UnsafeMutablePointer&lt;CFData?>) -> OSStatus

Creates a persistent reference for a keychain item.

Deprecated

func SecKeychainItemCopyFromPersistentReference(CFData, UnsafeMutablePointer&lt;SecKeychainItem?>) -> OSStatus

Provides a keychain item reference, given a persistent reference.

Deprecated

enum SecItemClass

Specifies a keychain item’s class code.

### Legacy keychain item management

Use the functions in Keychain item search instead.

func SecKeychainItemCopyAttributesAndData(SecKeychainItem, UnsafeMutablePointer&lt;SecKeychainAttributeInfo>?, UnsafeMutablePointer&lt;SecItemClass>?, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;SecKeychainAttributeList>?>?, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>?) -> OSStatus

Retrieves the data and/or attributes stored in the given keychain item.

Deprecated

func SecKeychainItemModifyAttributesAndData(SecKeychainItem, UnsafePointer&lt;SecKeychainAttributeList>?, UInt32, UnsafeRawPointer?) -> OSStatus

Updates an existing keychain item after changing its attributes or data.

Deprecated

func SecKeychainItemFreeAttributesAndData(UnsafeMutablePointer&lt;SecKeychainAttributeList>?, UnsafeMutableRawPointer?) -> OSStatus

Releases the memory used by the keychain attribute list and/or the keychain data retrieved in a call to `SecKeychainItemCopyAttributesAndData`.

Deprecated

func SecKeychainItemCopyContent(SecKeychainItem, UnsafeMutablePointer&lt;SecItemClass>?, UnsafeMutablePointer&lt;SecKeychainAttributeList>?, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>?) -> OSStatus

Copies the data and attributes stored in the given keychain item.

Deprecated

func SecKeychainItemModifyContent(SecKeychainItem, UnsafePointer&lt;SecKeychainAttributeList>?, UInt32, UnsafeRawPointer?) -> OSStatus

Updates an existing keychain item after changing its attributes and/or data.

Deprecated

func SecKeychainItemFreeContent(UnsafeMutablePointer&lt;SecKeychainAttributeList>?, UnsafeMutableRawPointer?) -> OSStatus

Releases the memory used by the keychain attribute list and the keychain data retrieved in a call to the SecKeychainItemCopyContent(_:_:_:_:_:) function.

Deprecated

func SecKeychainItemCopyKeychain(SecKeychainItem, UnsafeMutablePointer&lt;SecKeychain?>) -> OSStatus

Returns the keychain object of a given keychain item.

Deprecated

func SecKeychainItemDelete(SecKeychainItem) -> OSStatus

Deletes a keychain item from the default keychain’s permanent data store.

Deprecated

typealias SecKeychainAttrType

The keychain attribute type.

struct SecKeychainAttribute

A structure that holds a single keychain attribute.

typealias SecKeychainAttributePtr

A pointer to a keychain attribute structure.

struct SecKeychainAttributeList

A list of keychain attributes.

### Legacy attribute info

Use the functions in Adding keychain items and Keychain item search instead.

func SecKeychainAttributeInfoForItemID(SecKeychain?, UInt32, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;SecKeychainAttributeInfo>?>) -> OSStatus

Obtains tags for all possible attributes of a given item class.

Deprecated

func SecKeychainFreeAttributeInfo(UnsafeMutablePointer&lt;SecKeychainAttributeInfo>) -> OSStatus

Releases the memory acquired by calling the `SecKeychainAttributeInfoForItemID` function.

Deprecated

struct SecKeychainAttributeInfo

A structure that represents an attribute.

enum SecItemAttr

Specifies a keychain item’s attributes.

Keychain Item Attribute Constants For Keys

Specifies the attributes for a key item in a keychain.

typealias SecAFPServerSignature

Represents a 16-byte Apple File Protocol server signature block.

Deprecated

### Legacy password storage

Use the functions in Adding keychain items and Keychain item search instead.

func SecKeychainAddInternetPassword(SecKeychain?, UInt32, UnsafePointer&lt;CChar>?, UInt32, UnsafePointer&lt;CChar>?, UInt32, UnsafePointer&lt;CChar>?, UInt32, UnsafePointer&lt;CChar>?, UInt16, SecProtocolType, SecAuthenticationType, UInt32, UnsafeRawPointer, UnsafeMutablePointer&lt;SecKeychainItem?>?) -> OSStatus

Adds a new Internet password to a keychain.

Deprecated

func SecKeychainFindInternetPassword(CFTypeRef?, UInt32, UnsafePointer&lt;CChar>?, UInt32, UnsafePointer&lt;CChar>?, UInt32, UnsafePointer&lt;CChar>?, UInt32, UnsafePointer&lt;CChar>?, UInt16, SecProtocolType, SecAuthenticationType, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>?, UnsafeMutablePointer&lt;SecKeychainItem?>?) -> OSStatus

Finds the first Internet password based on the attributes passed.

Deprecated

func SecKeychainAddGenericPassword(SecKeychain?, UInt32, UnsafePointer&lt;CChar>?, UInt32, UnsafePointer&lt;CChar>?, UInt32, UnsafeRawPointer, UnsafeMutablePointer&lt;SecKeychainItem?>?) -> OSStatus

Adds a new generic password to a keychain.

Deprecated

func SecKeychainFindGenericPassword(CFTypeRef?, UInt32, UnsafePointer&lt;CChar>?, UInt32, UnsafePointer&lt;CChar>?, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>?, UnsafeMutablePointer&lt;SecKeychainItem?>?) -> OSStatus

Finds the first generic password based on the attributes passed.

Deprecated

enum SecProtocolType

The protocol type associated with an Internet password.

enum SecAuthenticationType

The authentication type to use for an Internet password.

class SecPassword

Contains information about a password.

