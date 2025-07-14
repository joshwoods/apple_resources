

- AppKit
- NSDiffableDataSourceSnapshotReference
-  insertItems(withIdentifiers:beforeItemWithIdentifier:) 

Instance Method

# insertItems(withIdentifiers:beforeItemWithIdentifier:)

Inserts the provided items immediately before the item with the specified identifier in the snapshot.

macOS 10.15+

``` source
func insertItems(
    withIdentifiers identifiers: [Any],
    beforeItemWithIdentifier itemIdentifier: Any
)
```

## Parameters 

`identifiers`  

The array of identifiers corresponding to the items to add to the snapshot.

`itemIdentifier`  

The identifier of the item before which to insert the new items.

## See Also

### Inserting items and sections

func insertItems(withIdentifiers: [Any], afterItemWithIdentifier: Any)

Inserts the provided items immediately after the item with the specified identifier in the snapshot.

func insertSections(withIdentifiers: [Any], afterSectionWithIdentifier: Any)

Inserts the provided sections immediately after the section with the specified identifier in the snapshot.

func insertSections(withIdentifiers: [Any], beforeSectionWithIdentifier: Any)

Inserts the provided sections immediately before the section with the specified identifier in the snapshot.

