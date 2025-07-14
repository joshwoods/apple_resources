

- AppKit
- NSDiffableDataSourceSnapshot
-  itemIdentifiers(inSection:) 

Instance Method

# itemIdentifiers(inSection:)

Returns the identifiers of all of the items in the specified section of the snapshot.

macOS 10.15.1+

``` source
func itemIdentifiers(inSection identifier: SectionIdentifierType) -> [ItemIdentifierType]
```

## Parameters 

`identifier`  

The identifier of the section of the snapshot.

## Return Value

An array of identifiers of the items contained in the section.

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

func sectionIdentifier(containingItem: ItemIdentifierType) -> SectionIdentifierType?

Returns the identifier of the section containing the specified item in the snapshot.

