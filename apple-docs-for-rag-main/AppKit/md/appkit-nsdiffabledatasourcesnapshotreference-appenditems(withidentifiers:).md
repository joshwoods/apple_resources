

- AppKit
- NSDiffableDataSourceSnapshotReference
-  appendItems(withIdentifiers:) 

Instance Method

# appendItems(withIdentifiers:)

Adds the items with the specified identifiers to the last section of the snapshot.

macOS 10.15+

``` source
func appendItems(withIdentifiers identifiers: [Any])
```

## Parameters 

`identifiers`  

An array of identifiers specifying the items to add to the snapshot.

## See Also

### Creating a snapshot

func appendSections(withIdentifiers: [Any])

Adds the sections with the specified identifiers to the snapshot.

func appendItems(withIdentifiers: [Any], intoSectionWithIdentifier: Any)

Adds the items with the specified identifiers to the specified section of the snapshot.

