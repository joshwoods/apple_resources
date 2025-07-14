

- Authentication Services
-  ASImportableItem 

Structure

# ASImportableItem

An item for use in import and export.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
struct ASImportableItem
```

## Overview

An item represents an account for a service stored by the password manager. One item can store multiple credentials. For example, to represent an account with a password and a passkey, use an item with two credentials: a ASImportableCredential.BasicAuthentication password and a ASImportableCredential.Passkey.

This type is a representation of `Item` as defined in the Credential Exchange Format (CXF) specification. You can supply a JSON representation of a CXF `Item` to initialize an instance of this struct by using a JSONDecoder and calling decode(_:from:).

## Topics

### Creating an item

init(id: Data, created: Date, lastModified: Date, type: ASImportableItem.ItemType, title: String, subtitle: String?, credentials: [ASImportableCredential], tags: [String])

Creates an importable item.

### Accessing item properties

var id: Data

A unique identifier for the item.

var created: Date

The item’s creation date and time.

var lastModified: Date

The item’s last modified date and time.

var type: ASImportableItem.ItemType

The type of the item.

enum ItemType

The type of an importable item.

var subtitle: String?

A subtitle or description of this item, if any.

var credentials: [ASImportableCredential]

The credentials associated with this item.

enum ASImportableCredential

A credential for use in import and export.

var tags: [String]

The user-defined tags associated with this item, if any.

### Instance Properties

var title: String

The user-defined name or title of this item.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Accessing account properties

var id: Data

A unique identifier for the account.

var userName: String

The username associated with the account.

var email: String

The email address associated with this account.

var fullName: String?

The full name of the account owner, if provided.

var collections: [ASImportableCollection]

The collections stored in this account.

struct ASImportableCollection

A collection of items and subcollections for use in import and export.

var items: [ASImportableItem]

All items stored in the account.

