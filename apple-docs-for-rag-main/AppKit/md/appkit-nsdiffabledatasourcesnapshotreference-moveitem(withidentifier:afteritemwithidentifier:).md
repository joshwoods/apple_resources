

- AppKit
- NSDiffableDataSourceSnapshotReference
-  moveItem(withIdentifier:afterItemWithIdentifier:) 

Instance Method

# moveItem(withIdentifier:afterItemWithIdentifier:)

Moves the item from its current position in the snapshot to the position immediately after the specified item.

macOS 10.15+

``` source
func moveItem(
    withIdentifier fromIdentifier: Any,
    afterItemWithIdentifier toIdentifier: Any
)
```

## Parameters 

`fromIdentifier`  

The identifier of the item to move in the snapshot.

`toIdentifier`  

The identifier of the item after which to move the specified item.

## See Also

### Reordering items and sections

func moveItem(withIdentifier: Any, beforeItemWithIdentifier: Any)

Moves the item from its current position in the snapshot to the position immediately before the specified item.

func moveSection(withIdentifier: Any, afterSectionWithIdentifier: Any)

Moves the section from its current position in the snapshot to the position immediately after the specified section.

func moveSection(withIdentifier: Any, beforeSectionWithIdentifier: Any)

Moves the section from its current position in the snapshot to the position immediately before the specified section.

