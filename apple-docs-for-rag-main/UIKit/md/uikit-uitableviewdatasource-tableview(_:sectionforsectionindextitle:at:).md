

- UIKit
- UITableViewDataSource
-  tableView(\_:sectionForSectionIndexTitle:at:) 

Instance Method

# tableView(\_:sectionForSectionIndexTitle:at:)

Asks the data source to return the index of the section having the given title and section title index.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    sectionForSectionIndexTitle title: String,
    at index: Int
) -> Int
```

## Parameters 

`tableView`  

The table-view object requesting this information.

`title`  

The title as displayed in the section index of `tableView`.

`index`  

An index number identifying a section title in the array returned by sectionIndexTitles(for:).

## Return Value

An index number identifying a section.

## Discussion

This method is passed the index number and title of an entry in the section index list and should return the index of the referenced section. To be clear, there are two index numbers in play here: an index to a section index title in the array returned by sectionIndexTitles(for:), and an index to a section of the table view; the former is passed in, and the latter is returned. You implement this method only for table views with a section index list — which can only be table views created in the plain style (UITableView.Style.plain). Note that the array of section titles returned by sectionIndexTitles(for:) can have fewer items than the actual number of sections in the table view.

## See Also

### Related Documentation

func numberOfSections(in: UITableView) -> Int

Asks the data source to return the number of sections in the table view.

### Configuring an index

func sectionIndexTitles(for: UITableView) -> [String]?

Asks the data source to return the titles for the sections of a table view.

