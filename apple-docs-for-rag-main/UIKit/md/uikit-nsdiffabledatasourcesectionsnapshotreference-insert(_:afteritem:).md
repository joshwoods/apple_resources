

- UIKit
- NSDiffableDataSourceSectionSnapshotReference
-  insert(\_:afterItem:) 

Instance Method

# insert(\_:afterItem:)

Inserts the provided section snapshot immediately after the item with the specified identifier in the section snapshot.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
func insert(
    _ snapshot: NSDiffableDataSourceSectionSnapshotReference,
    afterItem item: Any
) -> Any
```

## See Also

### Inserting items

func insertItems([Any], afterItem: Any)

Inserts the provided items immediately after the item with the specified identifier in the section snapshot.

func insert(NSDiffableDataSourceSectionSnapshotReference, beforeItem: Any)

Inserts the provided section snapshot immediately before the item with the specified identifier in the section snapshot.

func insertItems([Any], beforeItem: Any)

Inserts the provided items immediately before the item with the specified identifier in the section snapshot.

