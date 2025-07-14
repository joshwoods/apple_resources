

- AppKit
- NSDiffableDataSourceSnapshot
-  indexOfItem(\_:) 

Instance Method

# indexOfItem(\_:)

Returns the index of the item in the snapshot with the specified identifier.

macOS 10.15.1+

``` source
func indexOfItem(_ identifier: ItemIdentifierType) -> Int?
```

## Parameters 

`identifier`  

The identifier of the item in the snapshot.

## Return Value

The index of the item in the snapshot, or `nil` if the item with the specified identifier doesn’t exist in the snapshot. This index value is 0-based.

## See Also

### Identifying Items and Sections

var itemIdentifiers: [ItemIdentifierType]

The identifiers of all of the items in the snapshot.

var sectionIdentifiers: [SectionIdentifierType]

The identifiers of all of the sections in the snapshot.

func indexOfSection(SectionIdentifierType) -> Int?

Returns the index of the section of the snapshot with the specified identifier.

func itemIdentifiers(inSection: SectionIdentifierType) -> [ItemIdentifierType]

Returns the identifiers of all of the items in the specified section of the snapshot.

func sectionIdentifier(containingItem: ItemIdentifierType) -> SectionIdentifierType?

Returns the identifier of the section containing the specified item in the snapshot.

