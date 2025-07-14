

- UIKit
- NSDiffableDataSourceSnapshot
-  indexOfSection(\_:) 

Instance Method

# indexOfSection(\_:)

Returns the index of the section of the snapshot with the specified identifier.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 13.0+visionOS

``` source
func indexOfSection(_ identifier: SectionIdentifierType) -> Int?
```

## Parameters 

`identifier`  

The identifier of the section of the snapshot.

## Return Value

The index of the section of the snapshot, or `nil` if the section with the specified identifier doesn’t exist in the snapshot. This index value is 0-based.

## See Also

### Identifying items and sections

var itemIdentifiers: [ItemIdentifierType]

The identifiers of all of the items in the snapshot.

var sectionIdentifiers: [SectionIdentifierType]

The identifiers of all of the sections in the snapshot.

func indexOfItem(ItemIdentifierType) -> Int?

Returns the index of the item in the snapshot with the specified identifier.

func itemIdentifiers(inSection: SectionIdentifierType) -> [ItemIdentifierType]

Returns the identifiers of all of the items in the specified section of the snapshot.

func sectionIdentifier(containingItem: ItemIdentifierType) -> SectionIdentifierType?

Returns the identifier of the section containing the specified item in the snapshot.

