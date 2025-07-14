

- AppKit
- NSTableViewDiffableDataSource
-  sectionIdentifier(forRow:) 

Instance Method

# sectionIdentifier(forRow:)

Returns the identifier of the section containing the specified row in the snapshot.

macOS 11.0+

``` source
func sectionIdentifier(forRow row: Int) -> SectionIdentifierType?
```

## Parameters 

`row`  

The row of the section in the table view.

## Return Value

The section’s identifier, or `nil` if the method doesn’t find an item with the provided item identifier.

## See Also

### Identifying Items and Sections

func itemIdentifier(forRow: Int) -> ItemIdentifierType?

Returns an identifier for the item at the specified row in the table view.

func row(forItemIdentifier: ItemIdentifierType) -> Int?

Returns a row for the item with the specified identifier in the table view.

func row(forSectionIdentifier: SectionIdentifierType) -> Int?

Returns a row for the section with the specified identifier in the table view.

