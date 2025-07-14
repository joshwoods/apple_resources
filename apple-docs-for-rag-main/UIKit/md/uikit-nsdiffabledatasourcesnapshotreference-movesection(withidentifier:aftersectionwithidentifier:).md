

- UIKit
- NSDiffableDataSourceSnapshotReference
-  moveSection(withIdentifier:afterSectionWithIdentifier:) 

Instance Method

# moveSection(withIdentifier:afterSectionWithIdentifier:)

Moves the section from its current position in the snapshot to the position immediately after the specified section.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
func moveSection(
    withIdentifier fromSectionIdentifier: Any,
    afterSectionWithIdentifier toSectionIdentifier: Any
)
```

## Parameters 

`fromSectionIdentifier`  

The identifier of the section to move in the snapshot.

`toSectionIdentifier`  

The identifier of the section after which to move the specified section.

## See Also

### Reordering items and sections

func moveItem(withIdentifier: Any, afterItemWithIdentifier: Any)

Moves the item from its current position in the snapshot to the position immediately after the specified item.

func moveItem(withIdentifier: Any, beforeItemWithIdentifier: Any)

Moves the item from its current position in the snapshot to the position immediately before the specified item.

func moveSection(withIdentifier: Any, beforeSectionWithIdentifier: Any)

Moves the section from its current position in the snapshot to the position immediately before the specified section.

