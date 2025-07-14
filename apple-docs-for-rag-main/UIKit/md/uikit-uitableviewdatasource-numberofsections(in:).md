

- UIKit
- UITableViewDataSource
-  numberOfSections(in:) 

Instance Method

# numberOfSections(in:)

Asks the data source to return the number of sections in the table view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func numberOfSections(in tableView: UITableView) -> Int
```

## Parameters 

`tableView`  

An object representing the table view requesting this information.

## Return Value

The number of sections in `tableView`.

## Discussion

If you don’t implement this method, the table configures the table with one section.

## See Also

### Providing the number of rows and sections

func tableView(UITableView, numberOfRowsInSection: Int) -> Int

Tells the data source to return the number of rows in a given section of a table view.

**Required**

