

- UIKit
- NSDiffableDataSourceSectionSnapshot
-  snapshot(of:includingParent:) 

Instance Method

# snapshot(of:includingParent:)

Creates a section snapshot that contains the child items of the specified parent item, optionally including the parent item.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
func snapshot(
    of parent: ItemIdentifierType,
    includingParent: Bool = false
) -> NSDiffableDataSourceSectionSnapshot
```

## See Also

### Creating a section snapshot

init()

Creates an empty section snapshot.

init(NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>)

Creates a copy of the provided section snapshot.

func append([ItemIdentifierType], to: ItemIdentifierType?)

Adds the specified items as child items of the specified parent item in the section snapshot.

