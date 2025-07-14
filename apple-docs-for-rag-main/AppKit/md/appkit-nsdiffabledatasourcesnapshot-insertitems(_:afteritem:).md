

- AppKit
- NSDiffableDataSourceSnapshot
-  insertItems(\_:afterItem:) 

Instance Method

# insertItems(\_:afterItem:)

Inserts the provided items immediately after the item with the specified identifier in the snapshot.

macOS 10.15.1+

``` source
mutating func insertItems(
    _ identifiers: [ItemIdentifierType],
    afterItem afterIdentifier: ItemIdentifierType
)
```

## Parameters 

`identifiers`  

The array of identifiers corresponding to the items to add to the snapshot.

`afterIdentifier`  

The identifier of the item after which to insert the new items.

## See Also

### Inserting Items and Sections

func insertItems([ItemIdentifierType], beforeItem: ItemIdentifierType)

Inserts the provided items immediately before the item with the specified identifier in the snapshot.

func insertSections([SectionIdentifierType], afterSection: SectionIdentifierType)

Inserts the provided sections immediately after the section with the specified identifier in the snapshot.

func insertSections([SectionIdentifierType], beforeSection: SectionIdentifierType)

Inserts the provided sections immediately before the section with the specified identifier in the snapshot.

