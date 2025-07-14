

- UIKit
- NSDiffableDataSourceSectionSnapshot
-  init(\_:) 

Initializer

# init(\_:)

Creates a copy of the provided section snapshot.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
init(_ snapshot: NSDiffableDataSourceSectionSnapshot)
```

## See Also

### Creating a section snapshot

init()

Creates an empty section snapshot.

func snapshot(of: ItemIdentifierType, includingParent: Bool) -> NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>

Creates a section snapshot that contains the child items of the specified parent item, optionally including the parent item.

func append([ItemIdentifierType], to: ItemIdentifierType?)

Adds the specified items as child items of the specified parent item in the section snapshot.

