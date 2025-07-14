

- UIKit
- NSDiffableDataSourceSnapshot
-  moveSection(\_:beforeSection:) 

Instance Method

# moveSection(\_:beforeSection:)

Moves the section from its current position in the snapshot to the position immediately before the specified section.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 13.0+visionOS

``` source
mutating func moveSection(
    _ identifier: SectionIdentifierType,
    beforeSection toIdentifier: SectionIdentifierType
)
```

## Parameters 

`identifier`  

The identifier of the section to move in the snapshot.

`toIdentifier`  

The identifier of the section before which to move the specified section.

## See Also

### Reordering items and sections

func moveItem(ItemIdentifierType, afterItem: ItemIdentifierType)

Moves the item from its current position in the snapshot to the position immediately after the specified item.

func moveItem(ItemIdentifierType, beforeItem: ItemIdentifierType)

Moves the item from its current position in the snapshot to the position immediately before the specified item.

func moveSection(SectionIdentifierType, afterSection: SectionIdentifierType)

Moves the section from its current position in the snapshot to the position immediately after the specified section.

