

- Authentication Services
-  ASImportableCollection 

Structure

# ASImportableCollection

A collection of items and subcollections for use in import and export.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
struct ASImportableCollection
```

## Overview

A collection represents a group of items such as a vault or folder.

This type is a representation of `Collection` as defined in the Credential Exchange Format (CXF) specification. You can supply a JSON representation of a CXF `Collection` to initialize an instance of this struct by using a JSONDecoder and calling decode(_:from:).

## Topics

### Creating a collection

init(id: Data, title: String, subtitle: String?, items: [ASImportableLinkedItem], subcollections: [ASImportableCollection])

Creates a collection from its items, child collections, and identifying information.

### Accessing collection properties

var id: Data

A unique identifier for the collection.

var title: String

The title of the collection.

var subtitle: String?

The subtitle of the collection, if any.

var items: [ASImportableLinkedItem]

The items that are part of the collection.

struct ASImportableLinkedItem

A linked item for use in import and export.

var subcollections: [ASImportableCollection]

Subcollections that are part of the collection.

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

var items: [ASImportableItem]

All items stored in the account.

struct ASImportableItem

An item for use in import and export.

