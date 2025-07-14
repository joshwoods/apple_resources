

- UIKit
- UITableViewDataSource
-  sectionIndexTitles(for:) 

Instance Method

# sectionIndexTitles(for:)

Asks the data source to return the titles for the sections of a table view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func sectionIndexTitles(for tableView: UITableView) -> [String]?
```

## Parameters 

`tableView`  

The table-view object requesting this information.

## Return Value

An array of strings that serve as the title of sections in the table view and appear in the index list on the right side of the table view. The table view must be in the plain style (`UITableViewStylePlain`). For example, for an alphabetized list, you could return an array containing strings “A” through “Z”.

## See Also

### Configuring an index

func tableView(UITableView, sectionForSectionIndexTitle: String, at: Int) -> Int

Asks the data source to return the index of the section having the given title and section title index.

