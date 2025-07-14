

- UIKit
- NSDiffableDataSourceSectionSnapshotReference
-  ofParentItem(\_:) 

Instance Method

# ofParentItem(\_:)

Creates a section snapshot containing the child items of the specified parent item, excluding the parent item.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
func ofParentItem(_ parentItem: Any) -> NSDiffableDataSourceSectionSnapshotReference
```

## See Also

### Creating a section snapshot

init()

Creates an empty section snapshot.

func ofParentItem(Any, includingParentItem: Bool) -> NSDiffableDataSourceSectionSnapshotReference

Creates a section snapshot containing the child items of the specified parent item, including the parent item.

func appendItems([Any])

Adds the specified items to the section snapshot.

func appendItems([Any], intoParentItem: Any?)

Adds the specified items as child items of the specified parent item in the section snapshot.

