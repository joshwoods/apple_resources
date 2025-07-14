

- UIKit
- NSDiffableDataSourceSnapshot
-  appendItems(\_:toSection:) 

Instance Method

# appendItems(\_:toSection:)

Adds the items with the specified identifiers to the specified section of the snapshot.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 13.0+visionOS

``` source
mutating func appendItems(
    _ identifiers: [ItemIdentifierType],
    toSection sectionIdentifier: SectionIdentifierType? = nil
)
```

## Parameters 

`identifiers`  

An array of identifiers specifying the items to add to the snapshot.

`sectionIdentifier`  

The section to which to add the items. If no value is provided, the items are appended to the last section of the snapshot.

## See Also

### Creating a snapshot

init()

Creates an empty snapshot.

func appendSections([SectionIdentifierType])

Adds the sections with the specified identifiers to the snapshot.

