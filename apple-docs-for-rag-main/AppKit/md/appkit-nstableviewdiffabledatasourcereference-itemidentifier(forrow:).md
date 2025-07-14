

- AppKit
- NSTableViewDiffableDataSourceReference
-  itemIdentifier(forRow:) 

Instance Method

# itemIdentifier(forRow:)

Returns an identifier for the item at the specified row in the table view.

macOS 11.0+

``` source
func itemIdentifier(forRow row: Int) -> ItemIdentifierType?
```

## Parameters 

`row`  

The row of the item in the table view.

## Return Value

The item’s identifier, or `nil` if the method doesn’t find an item at the provided row.

## See Also

### Identifying Items and Sections

func row(forItemIdentifier: ItemIdentifierType) -> Int

Returns a row for the item with the specified identifier in the table view.

func sectionIdentifier(forRow: Int) -> SectionIdentifierType?

Returns the identifier of the section containing the specified row in the snapshot.

func row(forSectionIdentifier: SectionIdentifierType) -> Int

Returns a row for the section with the specified identifier in the table view.

