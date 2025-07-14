

- AppKit
- NSDiffableDataSourceSnapshot
-  deleteSections(\_:) 

Instance Method

# deleteSections(\_:)

Deletes the sections with the specified identifiers from the snapshot.

macOS 10.15.1+

``` source
mutating func deleteSections(_ identifiers: [SectionIdentifierType])
```

## Parameters 

`identifiers`  

The array of identifiers corresponding to the sections to delete from the snapshot.

## See Also

### Removing Items and Sections

func deleteAllItems()

Deletes all of the items from the snapshot.

func deleteItems([ItemIdentifierType])

Deletes the items with the specified identifiers from the snapshot.

