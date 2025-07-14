

- UIKit
- NSDiffableDataSourceSnapshotReference
-  moveItem(withIdentifier:beforeItemWithIdentifier:) 

Instance Method

# moveItem(withIdentifier:beforeItemWithIdentifier:)

Moves the item from its current position in the snapshot to the position immediately before the specified item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
func moveItem(
    withIdentifier fromIdentifier: Any,
    beforeItemWithIdentifier toIdentifier: Any
)
```

## Parameters 

`fromIdentifier`  

The identifier of the item to move in the snapshot.

`toIdentifier`  

The identifier of the item before which to move the specified item.

## See Also

### Reordering items and sections

func moveItem(withIdentifier: Any, afterItemWithIdentifier: Any)

Moves the item from its current position in the snapshot to the position immediately after the specified item.

func moveSection(withIdentifier: Any, afterSectionWithIdentifier: Any)

Moves the section from its current position in the snapshot to the position immediately after the specified section.

func moveSection(withIdentifier: Any, beforeSectionWithIdentifier: Any)

Moves the section from its current position in the snapshot to the position immediately before the specified section.

