

- AppKit
- NSDiffableDataSourceSnapshot
-  appendSections(\_:) 

Instance Method

# appendSections(\_:)

Adds the sections with the specified identifiers to the snapshot.

macOS 10.15.1+

``` source
mutating func appendSections(_ identifiers: [SectionIdentifierType])
```

## Parameters 

`identifiers`  

An array of identifiers specifying the sections to add to the snapshot.

## See Also

### Creating a Snapshot

init()

Creates an empty snapshot.

func appendItems([ItemIdentifierType], toSection: SectionIdentifierType?)

Adds the items with the specified identifiers to the specified section of the snapshot.

