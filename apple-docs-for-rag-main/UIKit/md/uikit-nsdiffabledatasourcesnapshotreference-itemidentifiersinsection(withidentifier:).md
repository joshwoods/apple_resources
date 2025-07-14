

- UIKit
- NSDiffableDataSourceSnapshotReference
-  itemIdentifiersInSection(withIdentifier:) 

Instance Method

# itemIdentifiersInSection(withIdentifier:)

Returns the identifiers of all of the items in the specified section of the snapshot.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
func itemIdentifiersInSection(withIdentifier sectionIdentifier: Any) -> [Any]
```

## Parameters 

`sectionIdentifier`  

The identifier of the section of the snapshot.

## Return Value

An array of identifiers of the items contained in the section.

## See Also

### Identifying items and sections

var itemIdentifiers: [Any]

The identifiers of all of the items in the snapshot.

var sectionIdentifiers: [Any]

The identifiers of all of the sections in the snapshot.

func index(ofItemIdentifier: Any) -> Int

Returns the index of the item in the snapshot with the specified identifier.

func index(ofSectionIdentifier: Any) -> Int

Returns the index of the section of the snapshot with the specified identifier.

func sectionIdentifier(forSectionContainingItemIdentifier: Any) -> Any?

Returns the identifier of the section containing the specified item in the snapshot.

