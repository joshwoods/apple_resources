

- AppKit
- NSDiffableDataSourceSnapshotReference
-  moveSection(withIdentifier:beforeSectionWithIdentifier:) 

Instance Method

# moveSection(withIdentifier:beforeSectionWithIdentifier:)

Moves the section from its current position in the snapshot to the position immediately before the specified section.

macOS 10.15+

``` source
func moveSection(
    withIdentifier fromSectionIdentifier: Any,
    beforeSectionWithIdentifier toSectionIdentifier: Any
)
```

## Parameters 

`fromSectionIdentifier`  

The identifier of the section to move in the snapshot.

`toSectionIdentifier`  

The identifier of the section before which to move the specified section.

## See Also

### Reordering items and sections

func moveItem(withIdentifier: Any, afterItemWithIdentifier: Any)

Moves the item from its current position in the snapshot to the position immediately after the specified item.

func moveItem(withIdentifier: Any, beforeItemWithIdentifier: Any)

Moves the item from its current position in the snapshot to the position immediately before the specified item.

func moveSection(withIdentifier: Any, afterSectionWithIdentifier: Any)

Moves the section from its current position in the snapshot to the position immediately after the specified section.

