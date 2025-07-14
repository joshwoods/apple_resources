

- Authentication Services
- ASImportableItem
-  tags 

Instance Property

# tags

The user-defined tags associated with this item, if any.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
var tags: [String]
```

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

enum ItemType

The type of an importable item.

var subtitle: String?

A subtitle or description of this item, if any.

var credentials: [ASImportableCredential]

The credentials associated with this item.

enum ASImportableCredential

A credential for use in import and export.

