

- UIKit
- NSDiffableDataSourceSectionSnapshotReference
-  appendItems(\_:intoParentItem:) 

Instance Method

# appendItems(\_:intoParentItem:)

Adds the specified items as child items of the specified parent item in the section snapshot.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
func appendItems(
    _ items: [Any],
    intoParentItem parentItem: Any?
)
```

## Parameters 

`items`  

The identifiers of the items to append to the parent item in the section snapshot.

`parentItem`  

The parent item to append the items to.

## See Also

### Creating a section snapshot

init()

Creates an empty section snapshot.

func ofParentItem(Any) -> NSDiffableDataSourceSectionSnapshotReference

Creates a section snapshot containing the child items of the specified parent item, excluding the parent item.

func ofParentItem(Any, includingParentItem: Bool) -> NSDiffableDataSourceSectionSnapshotReference

Creates a section snapshot containing the child items of the specified parent item, including the parent item.

func appendItems([Any])

Adds the specified items to the section snapshot.

