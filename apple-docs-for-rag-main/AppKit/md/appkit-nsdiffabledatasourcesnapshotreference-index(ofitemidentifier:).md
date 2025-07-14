

- AppKit
- NSDiffableDataSourceSnapshotReference
-  index(ofItemIdentifier:) 

Instance Method

# index(ofItemIdentifier:)

Returns the index of the item in the snapshot with the specified identifier.

macOS 10.15+

``` source
func index(ofItemIdentifier itemIdentifier: Any) -> Int
```

## Parameters 

`itemIdentifier`  

The identifier of the item in the snapshot.

## Return Value

The index of the item in the snapshot, or `NSNotFound` if the item with the specified identifier doesn’t exist in the snapshot. This index value is 0-based.

## See Also

### Identifying items and sections

var itemIdentifiers: [Any]

The identifiers of all of the items in the snapshot.

var sectionIdentifiers: [Any]

The identifiers of all of the sections in the snapshot.

func index(ofSectionIdentifier: Any) -> Int

Returns the index of the section of the snapshot with the specified identifier.

func itemIdentifiersInSection(withIdentifier: Any) -> [Any]

Returns the identifiers of all of the items in the specified section of the snapshot.

func sectionIdentifier(forSectionContainingItemIdentifier: Any) -> Any?

Returns the identifier of the section containing the specified item in the snapshot.

