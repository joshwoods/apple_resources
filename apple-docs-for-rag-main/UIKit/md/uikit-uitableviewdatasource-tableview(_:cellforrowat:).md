

- UIKit
- UITableViewDataSource
-  tableView(\_:cellForRowAt:) 

Instance Method

# tableView(\_:cellForRowAt:)

Asks the data source for a cell to insert in a particular location of the table view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func tableView(
    _ tableView: UITableView,
    cellForRowAt indexPath: IndexPath
) -> UITableViewCell
```

**Required**

## Parameters 

`tableView`  

A table-view object requesting the cell.

`indexPath`  

An index path locating a row in `tableView`.

## Return Value

An object inheriting from UITableViewCell that the table view can use for the specified row. UIKit raises an assertion if you return `nil`.

## Mentioned in 

Configuring the cells for your table

Filling a table with data

## Discussion

In your implementation, create and configure an appropriate cell for the given index path. Create your cell using the table view’s dequeueReusableCell(withIdentifier:for:) method, which recycles or creates the cell for you. After creating the cell, update the properties of the cell with appropriate data values.

Never call this method yourself. If you want to retrieve cells from your table, call the table view’s cellForRow(at:) method instead.

## See Also

### Providing cells, headers, and footers

func tableView(UITableView, titleForHeaderInSection: Int) -> String?

Asks the data source for the title of the header of the specified section of the table view.

func tableView(UITableView, titleForFooterInSection: Int) -> String?

Asks the data source for the title of the footer of the specified section of the table view.

