

- Authentication Services
- ASImportableCollection
-  id 

Instance Property

# id

A unique identifier for the collection.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
var id: Data
```

## Discussion

This property isn’t displayed to the person using the app.

## See Also

### Accessing collection properties

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

