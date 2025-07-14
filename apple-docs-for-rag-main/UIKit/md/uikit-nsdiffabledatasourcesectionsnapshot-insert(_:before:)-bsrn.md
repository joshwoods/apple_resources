

- UIKit
- NSDiffableDataSourceSectionSnapshot
-  insert(\_:before:) 

Instance Method

# insert(\_:before:)

Inserts the provided section snapshot immediately before the item with the specified identifier in the section snapshot.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
mutating func insert(
    _ snapshot: NSDiffableDataSourceSectionSnapshot,
    before item: ItemIdentifierType
)
```

## See Also

### Inserting items

func insert([ItemIdentifierType], after: ItemIdentifierType)

Inserts the provided items immediately after the item with the specified identifier in the section snapshot.

func insert(NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>, after: ItemIdentifierType)

Inserts the provided section snapshot immediately after the item with the specified identifier in the section snapshot.

func insert([ItemIdentifierType], before: ItemIdentifierType)

Inserts the provided items immediately before the item with the specified identifier in the section snapshot.

