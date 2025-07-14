

- Authentication Services
- ASImportableCollection
-  init(id:title:subtitle:items:subcollections:) 

Initializer

# init(id:title:subtitle:items:subcollections:)

Creates a collection from its items, child collections, and identifying information.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
init(
    id: Data,
    title: String,
    subtitle: String? = nil,
    items: [ASImportableLinkedItem],
    subcollections: [ASImportableCollection] = []
)
```

## Parameters 

`id`  

A unique identifier for the collection.

`title`  

The title of the collection.

`subtitle`  

The subtitle of the collection, if any. Defaults to `nil`.

`items`  

The items that are part of the collection.

`subcollections`  

The child collections that are part of the collection. Defaults to an empty array.

