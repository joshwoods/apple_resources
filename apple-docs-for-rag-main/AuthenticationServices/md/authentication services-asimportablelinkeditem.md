

- Authentication Services
-  ASImportableLinkedItem 

Structure

# ASImportableLinkedItem

A linked item for use in import and export.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
struct ASImportableLinkedItem
```

## Overview

A linked item serves as a reference to an item, and contains no data of its own.

This type is a representation of `LinkedItem` as defined in the Credential Exchange Format (CXF) specification. You can supply a JSON representation of a CXF `Item` to initialize an instance of this struct by using a JSONDecoder and calling decode(_:from:).

## Topics

### Creating a linked item

init(item: Data, account: Data?)

Creates a linked item from the identifiers of an item and an account.

### Accessing linked item properties

var item: Data

The unique identifier of the item linked by this linked item.

var account: Data?

The unique identifier of the account, if any, to which the linked item belongs.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Accessing collection properties

var id: Data

A unique identifier for the collection.

var title: String

The title of the collection.

var subtitle: String?

The subtitle of the collection, if any.

var items: [ASImportableLinkedItem]

The items that are part of the collection.

var subcollections: [ASImportableCollection]

Subcollections that are part of the collection.

