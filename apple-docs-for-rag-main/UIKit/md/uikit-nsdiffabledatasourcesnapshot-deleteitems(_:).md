

- UIKit
- NSDiffableDataSourceSnapshot
-  deleteItems(\_:) 

Instance Method

# deleteItems(\_:)

Deletes the items with the specified identifiers from the snapshot.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 13.0+visionOS

``` source
mutating func deleteItems(_ identifiers: [ItemIdentifierType])
```

## Parameters 

`identifiers`  

The array of identifiers corresponding to the items to delete from the snapshot.

## See Also

### Removing items and sections

func deleteAllItems()

Deletes all of the items from the snapshot.

func deleteSections([SectionIdentifierType])

Deletes the sections with the specified identifiers from the snapshot.

