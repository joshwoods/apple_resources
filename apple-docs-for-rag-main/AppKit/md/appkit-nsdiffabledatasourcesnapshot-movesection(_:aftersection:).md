

- AppKit
- NSDiffableDataSourceSnapshot
-  moveSection(\_:afterSection:) 

Instance Method

# moveSection(\_:afterSection:)

Moves the section from its current position in the snapshot to the position immediately after the specified section.

macOS 10.15.1+

``` source
mutating func moveSection(
    _ identifier: SectionIdentifierType,
    afterSection toIdentifier: SectionIdentifierType
)
```

## Parameters 

`identifier`  

The identifier of the section to move in the snapshot.

`toIdentifier`  

The identifier of the section after which to move the specified section.

## See Also

### Reordering Items and Sections

func moveItem(ItemIdentifierType, afterItem: ItemIdentifierType)

Moves the item from its current position in the snapshot to the position immediately after the specified item.

func moveItem(ItemIdentifierType, beforeItem: ItemIdentifierType)

Moves the item from its current position in the snapshot to the position immediately before the specified item.

func moveSection(SectionIdentifierType, beforeSection: SectionIdentifierType)

Moves the section from its current position in the snapshot to the position immediately before the specified section.

