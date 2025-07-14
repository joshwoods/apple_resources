

- AppKit
- NSDiffableDataSourceSnapshot
-  deleteItems(\_:) 

Instance Method

# deleteItems(\_:)

Deletes the items with the specified identifiers from the snapshot.

macOS 10.15.1+

``` source
mutating func deleteItems(_ identifiers: [ItemIdentifierType])
```

## Parameters 

`identifiers`  

The array of identifiers corresponding to the items to delete from the snapshot.

## See Also

### Removing Items and Sections

func deleteAllItems()

Deletes all of the items from the snapshot.

func deleteSections([SectionIdentifierType])

Deletes the sections with the specified identifiers from the snapshot.

