

- UIKit
- UILocalizedIndexedCollation
-  section(forSectionIndexTitle:) 

Instance Method

# section(forSectionIndexTitle:)

Returns the section that the table view should scroll to for the given index title.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func section(forSectionIndexTitle indexTitleIndex: Int) -> Int
```

## Parameters 

`indexTitleIndex`  

An integer identifying a section-index title by its position in the array of such titles.

## Return Value

An integer identifying the table-view section associated with `indexTitleIndex`.

## Discussion

This method allows the table view to map between a given item in the section index and a given section even when there isn’t a one-to-one mapping. In its implementation of tableView(_:sectionForSectionIndexTitle:at:), the data source can call this method on the indexed-collation object specifying as an argument the passed-in index integer; it then returns the result to the table view.

## See Also

### Providing section index data to the table view

var sectionTitles: [String]

Returns the list of section titles for the table view.

var sectionIndexTitles: [String]

Returns the list of section-index titles for the table view.

