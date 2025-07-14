

- Authentication Services
- ASImportableItem
-  ASImportableItem.ItemType 

Enumeration

# ASImportableItem.ItemType

The type of an importable item.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
enum ItemType
```

## Topics

### Item types

case login

The type for an item that contains login-related credential information.

case document

The type for an item that contains document-related credential information.

case identity

The type for an item that contains identity-related credential information.

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing item properties

var id: Data

A unique identifier for the item.

var created: Date

The item’s creation date and time.

var lastModified: Date

The item’s last modified date and time.

var type: ASImportableItem.ItemType

The type of the item.

var subtitle: String?

A subtitle or description of this item, if any.

var credentials: [ASImportableCredential]

The credentials associated with this item.

enum ASImportableCredential

A credential for use in import and export.

var tags: [String]

The user-defined tags associated with this item, if any.

