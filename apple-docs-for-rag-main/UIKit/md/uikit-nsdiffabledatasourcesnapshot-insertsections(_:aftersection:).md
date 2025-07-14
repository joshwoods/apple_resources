

- UIKit
- NSDiffableDataSourceSnapshot
-  insertSections(\_:afterSection:) 

Instance Method

# insertSections(\_:afterSection:)

Inserts the provided sections immediately after the section with the specified identifier in the snapshot.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 13.0+visionOS

``` source
mutating func insertSections(
    _ identifiers: [SectionIdentifierType],
    afterSection toIdentifier: SectionIdentifierType
)
```

## Parameters 

`identifiers`  

The array of identifiers corresponding to the sections to add to the snapshot.

`toIdentifier`  

The identifier of the section after which to insert the new sections.

## See Also

### Inserting items and sections

func insertItems([ItemIdentifierType], afterItem: ItemIdentifierType)

Inserts the provided items immediately after the item with the specified identifier in the snapshot.

func insertItems([ItemIdentifierType], beforeItem: ItemIdentifierType)

Inserts the provided items immediately before the item with the specified identifier in the snapshot.

func insertSections([SectionIdentifierType], beforeSection: SectionIdentifierType)

Inserts the provided sections immediately before the section with the specified identifier in the snapshot.

