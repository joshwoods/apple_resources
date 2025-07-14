

- UIKit
- NSDiffableDataSourceSnapshot
-  deleteSections(\_:) 

Instance Method

# deleteSections(\_:)

Deletes the sections with the specified identifiers from the snapshot.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 13.0+visionOS

``` source
mutating func deleteSections(_ identifiers: [SectionIdentifierType])
```

## Parameters 

`identifiers`  

The array of identifiers corresponding to the sections to delete from the snapshot.

## See Also

### Removing items and sections

func deleteAllItems()

Deletes all of the items from the snapshot.

func deleteItems([ItemIdentifierType])

Deletes the items with the specified identifiers from the snapshot.

