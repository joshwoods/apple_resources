

- UIKit
- NSDiffableDataSourceSnapshot
-  moveItem(\_:afterItem:) 

Instance Method

# moveItem(\_:afterItem:)

Moves the item from its current position in the snapshot to the position immediately after the specified item.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 13.0+visionOS

``` source
mutating func moveItem(
    _ identifier: ItemIdentifierType,
    afterItem toIdentifier: ItemIdentifierType
)
```

## Parameters 

`identifier`  

The identifier of the item to move in the snapshot.

`toIdentifier`  

The identifier of the item after which to move the specified item.

## See Also

### Reordering items and sections

func moveItem(ItemIdentifierType, beforeItem: ItemIdentifierType)

Moves the item from its current position in the snapshot to the position immediately before the specified item.

func moveSection(SectionIdentifierType, afterSection: SectionIdentifierType)

Moves the section from its current position in the snapshot to the position immediately after the specified section.

func moveSection(SectionIdentifierType, beforeSection: SectionIdentifierType)

Moves the section from its current position in the snapshot to the position immediately before the specified section.

