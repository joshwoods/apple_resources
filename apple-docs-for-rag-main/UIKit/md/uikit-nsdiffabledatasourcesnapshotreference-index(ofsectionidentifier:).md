

- UIKit
- NSDiffableDataSourceSnapshotReference
-  index(ofSectionIdentifier:) 

Instance Method

# index(ofSectionIdentifier:)

Returns the index of the section of the snapshot with the specified identifier.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
func index(ofSectionIdentifier sectionIdentifier: Any) -> Int
```

## Parameters 

`sectionIdentifier`  

The identifier of the section of the snapshot.

## Return Value

The index of the section of the snapshot, or `NSNotFound` if the section with the specified identifier doesn’t exist in the snapshot. This index value is 0-based.

## See Also

### Identifying items and sections

var itemIdentifiers: [Any]

The identifiers of all of the items in the snapshot.

var sectionIdentifiers: [Any]

The identifiers of all of the sections in the snapshot.

func index(ofItemIdentifier: Any) -> Int

Returns the index of the item in the snapshot with the specified identifier.

func itemIdentifiersInSection(withIdentifier: Any) -> [Any]

Returns the identifiers of all of the items in the specified section of the snapshot.

func sectionIdentifier(forSectionContainingItemIdentifier: Any) -> Any?

Returns the identifier of the section containing the specified item in the snapshot.

