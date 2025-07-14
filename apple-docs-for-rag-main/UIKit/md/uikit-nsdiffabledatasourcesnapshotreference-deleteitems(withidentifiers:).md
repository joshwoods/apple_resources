

- UIKit
- NSDiffableDataSourceSnapshotReference
-  deleteItems(withIdentifiers:) 

Instance Method

# deleteItems(withIdentifiers:)

Deletes the items with the specified identifiers from the snapshot.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
func deleteItems(withIdentifiers identifiers: [Any])
```

## Parameters 

`identifiers`  

The array of identifiers corresponding to the items to delete from the snapshot.

## See Also

### Removing items and sections

func deleteAllItems()

Deletes all of the items from the snapshot.

func deleteSections(withIdentifiers: [Any])

Deletes the sections with the specified identifiers from the snapshot.

