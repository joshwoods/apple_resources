

- AppKit
- NSTableViewDiffableDataSourceReference
-  row(forSectionIdentifier:) 

Instance Method

# row(forSectionIdentifier:)

Returns a row for the section with the specified identifier in the table view.

macOS 11.0+

``` source
func row(forSectionIdentifier identifier: SectionIdentifierType) -> Int
```

## Parameters 

`identifier`  

The identifier of the section in the table view.

## Return Value

The item’s section, or `nil` if the method doesn’t find an item with the provided item identifier.

## See Also

### Identifying Items and Sections

func itemIdentifier(forRow: Int) -> ItemIdentifierType?

Returns an identifier for the item at the specified row in the table view.

func row(forItemIdentifier: ItemIdentifierType) -> Int

Returns a row for the item with the specified identifier in the table view.

func sectionIdentifier(forRow: Int) -> SectionIdentifierType?

Returns the identifier of the section containing the specified row in the snapshot.

