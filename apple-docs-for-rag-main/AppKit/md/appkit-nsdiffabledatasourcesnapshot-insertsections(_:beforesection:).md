

- AppKit
- NSDiffableDataSourceSnapshot
-  insertSections(\_:beforeSection:) 

Instance Method

# insertSections(\_:beforeSection:)

Inserts the provided sections immediately before the section with the specified identifier in the snapshot.

macOS 10.15.1+

``` source
mutating func insertSections(
    _ identifiers: [SectionIdentifierType],
    beforeSection toIdentifier: SectionIdentifierType
)
```

## Parameters 

`identifiers`  

The array of identifiers corresponding to the sections to add to the snapshot.

`toIdentifier`  

The identifier of the section before which to insert the new sections.

## See Also

### Inserting Items and Sections

func insertItems([ItemIdentifierType], afterItem: ItemIdentifierType)

Inserts the provided items immediately after the item with the specified identifier in the snapshot.

func insertItems([ItemIdentifierType], beforeItem: ItemIdentifierType)

Inserts the provided items immediately before the item with the specified identifier in the snapshot.

func insertSections([SectionIdentifierType], afterSection: SectionIdentifierType)

Inserts the provided sections immediately after the section with the specified identifier in the snapshot.

