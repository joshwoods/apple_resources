

- UIKit
- NSDiffableDataSourceSnapshot
-  insertItems(\_:beforeItem:) 

Instance Method

# insertItems(\_:beforeItem:)

Inserts the provided items immediately before the item with the specified identifier in the snapshot.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 13.0+visionOS

``` source
mutating func insertItems(
    _ identifiers: [ItemIdentifierType],
    beforeItem beforeIdentifier: ItemIdentifierType
)
```

## Parameters 

`identifiers`  

The array of identifiers corresponding to the items to add to the snapshot.

`beforeIdentifier`  

The identifier of the item before which to insert the new items.

## See Also

### Inserting items and sections

func insertItems([ItemIdentifierType], afterItem: ItemIdentifierType)

Inserts the provided items immediately after the item with the specified identifier in the snapshot.

func insertSections([SectionIdentifierType], afterSection: SectionIdentifierType)

Inserts the provided sections immediately after the section with the specified identifier in the snapshot.

func insertSections([SectionIdentifierType], beforeSection: SectionIdentifierType)

Inserts the provided sections immediately before the section with the specified identifier in the snapshot.

