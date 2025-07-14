

- UIKit
- NSDiffableDataSourceSectionSnapshot
-  append(\_:to:) 

Instance Method

# append(\_:to:)

Adds the specified items as child items of the specified parent item in the section snapshot.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
mutating func append(
    _ items: [ItemIdentifierType],
    to parent: ItemIdentifierType? = nil
)
```

## Parameters 

`items`  

The identifiers of the items to append to the parent item in the section snapshot.

`parent`  

The parent item to append the items to. If you don’t specify a parent, the section snapshot appends the items to its root level.

## See Also

### Creating a section snapshot

init()

Creates an empty section snapshot.

init(NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>)

Creates a copy of the provided section snapshot.

func snapshot(of: ItemIdentifierType, includingParent: Bool) -> NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>

Creates a section snapshot that contains the child items of the specified parent item, optionally including the parent item.

