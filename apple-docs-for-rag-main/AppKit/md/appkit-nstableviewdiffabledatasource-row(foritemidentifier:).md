

- AppKit
- NSTableViewDiffableDataSource
-  row(forItemIdentifier:) 

Instance Method

# row(forItemIdentifier:)

Returns a row for the item with the specified identifier in the table view.

macOS 11.0+

``` source
func row(forItemIdentifier identifier: ItemIdentifierType) -> Int?
```

## Parameters 

`identifier`  

The identifier of the item in the table view.

## Return Value

The item’s row, or `nil` if the method doesn’t find an item with the provided item identifier.

## See Also

### Identifying Items and Sections

func itemIdentifier(forRow: Int) -> ItemIdentifierType?

Returns an identifier for the item at the specified row in the table view.

func sectionIdentifier(forRow: Int) -> SectionIdentifierType?

Returns the identifier of the section containing the specified row in the snapshot.

func row(forSectionIdentifier: SectionIdentifierType) -> Int?

Returns a row for the section with the specified identifier in the table view.

