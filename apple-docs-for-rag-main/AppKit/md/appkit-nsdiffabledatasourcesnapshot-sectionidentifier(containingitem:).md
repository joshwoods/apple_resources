

- AppKit
- NSDiffableDataSourceSnapshot
-  sectionIdentifier(containingItem:) 

Instance Method

# sectionIdentifier(containingItem:)

Returns the identifier of the section containing the specified item in the snapshot.

macOS 10.15.1+

``` source
func sectionIdentifier(containingItem identifier: ItemIdentifierType) -> SectionIdentifierType?
```

## Parameters 

`identifier`  

The identifier of the item contained in the section of the snapshot.

## Return Value

The identifier of the section containing the specified item, or `nil` if the specified item doesn’t exist in any section of the snapshot.

## See Also

### Identifying Items and Sections

var itemIdentifiers: [ItemIdentifierType]

The identifiers of all of the items in the snapshot.

var sectionIdentifiers: [SectionIdentifierType]

The identifiers of all of the sections in the snapshot.

func indexOfItem(ItemIdentifierType) -> Int?

Returns the index of the item in the snapshot with the specified identifier.

func indexOfSection(SectionIdentifierType) -> Int?

Returns the index of the section of the snapshot with the specified identifier.

func itemIdentifiers(inSection: SectionIdentifierType) -> [ItemIdentifierType]

Returns the identifiers of all of the items in the specified section of the snapshot.

