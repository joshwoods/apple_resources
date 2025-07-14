

- UIKit
- UITableViewDataSource
-  tableView(\_:canEditRowAt:) 

Instance Method

# tableView(\_:canEditRowAt:)

Asks the data source to verify that the given row is editable.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    canEditRowAt indexPath: IndexPath
) -> Bool
```

## Parameters 

`tableView`  

The table-view object requesting this information.

`indexPath`  

An index path locating a row in `tableView`.

## Return Value

true if the row indicated by `indexPath` is editable; otherwise, false.

## Discussion

The method permits the data source to exclude individual rows from being treated as editable. Editable rows display the insertion or deletion control in their cells. If this method isn’t implemented, all rows are assumed to be editable. Rows that aren’t editable ignore the editingStyle property of a `UITableViewCell` object and do no indentation for the deletion or insertion control. Rows that are editable, but that don’t want to have an insertion or remove control shown, can return UITableViewCell.EditingStyle.none from the tableView(_:editingStyleForRowAt:) delegate method.

## See Also

### Inserting or deleting table rows

func tableView(UITableView, commit: UITableViewCell.EditingStyle, forRowAt: IndexPath)

Asks the data source to commit the insertion or deletion of a specified row.

