

- UIKit
- NSDiffableDataSourceSnapshot
-  itemIdentifiers 

Instance Property

# itemIdentifiers

The identifiers of all of the items in the snapshot.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 13.0+visionOS

``` source
var itemIdentifiers: [ItemIdentifierType] { get }
```

## See Also

### Identifying items and sections

var sectionIdentifiers: [SectionIdentifierType]

The identifiers of all of the sections in the snapshot.

func indexOfItem(ItemIdentifierType) -> Int?

Returns the index of the item in the snapshot with the specified identifier.

func indexOfSection(SectionIdentifierType) -> Int?

Returns the index of the section of the snapshot with the specified identifier.

func itemIdentifiers(inSection: SectionIdentifierType) -> [ItemIdentifierType]

Returns the identifiers of all of the items in the specified section of the snapshot.

func sectionIdentifier(containingItem: ItemIdentifierType) -> SectionIdentifierType?

Returns the identifier of the section containing the specified item in the snapshot.

