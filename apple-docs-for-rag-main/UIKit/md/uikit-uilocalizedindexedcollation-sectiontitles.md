

- UIKit
- UILocalizedIndexedCollation
-  sectionTitles 

Instance Property

# sectionTitles

Returns the list of section titles for the table view.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var sectionTitles: [String] { get }
```

## Discussion

This property contains the localized list of section titles sorted according to the specified ordering (for example, A through Z in US English). In its implementation of tableView(_:titleForHeaderInSection:), the data source can call this method on the indexed-collation object, passing in the section index and returning the result.

## See Also

### Providing section index data to the table view

var sectionIndexTitles: [String]

Returns the list of section-index titles for the table view.

func section(forSectionIndexTitle: Int) -> Int

Returns the section that the table view should scroll to for the given index title.

