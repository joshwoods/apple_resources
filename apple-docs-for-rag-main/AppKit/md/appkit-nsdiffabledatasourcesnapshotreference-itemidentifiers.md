

- AppKit
- NSDiffableDataSourceSnapshotReference
-  itemIdentifiers 

Instance Property

# itemIdentifiers

The identifiers of all of the items in the snapshot.

macOS 10.15+

``` source
var itemIdentifiers: [Any] { get }
```

## See Also

### Identifying items and sections

var sectionIdentifiers: [Any]

The identifiers of all of the sections in the snapshot.

func index(ofItemIdentifier: Any) -> Int

Returns the index of the item in the snapshot with the specified identifier.

func index(ofSectionIdentifier: Any) -> Int

Returns the index of the section of the snapshot with the specified identifier.

func itemIdentifiersInSection(withIdentifier: Any) -> [Any]

Returns the identifiers of all of the items in the specified section of the snapshot.

func sectionIdentifier(forSectionContainingItemIdentifier: Any) -> Any?

Returns the identifier of the section containing the specified item in the snapshot.

