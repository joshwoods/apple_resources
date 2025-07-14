

- UIKit
- UITableViewDataSource
-  tableView(\_:numberOfRowsInSection:) 

Instance Method

# tableView(\_:numberOfRowsInSection:)

Tells the data source to return the number of rows in a given section of a table view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func tableView(
    _ tableView: UITableView,
    numberOfRowsInSection section: Int
) -> Int
```

**Required**

## Parameters 

`tableView`  

The table-view object requesting this information.

`section`  

An index number identifying a section in `tableView`.

## Return Value

The number of rows in `section`.

## See Also

### Providing the number of rows and sections

func numberOfSections(in: UITableView) -> Int

Asks the data source to return the number of sections in the table view.

