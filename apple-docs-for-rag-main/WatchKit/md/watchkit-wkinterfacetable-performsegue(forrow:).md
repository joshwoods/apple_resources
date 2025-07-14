

- WatchKit
- WKInterfaceTable
-  performSegue(forRow:) 

Instance Method

# performSegue(forRow:)

Performs the segue for the specified row.

watchOS 3.0+

``` source
func performSegue(forRow row: Int)
```

## Parameters 

`row`  

The index of the row.

## Discussion

This method lets you programmatically transition to a new interface controller. It triggers the segue defined in your storyboard file for the specified row controller.

While similar to the WKInterfaceController class’s pushController(withName:context:) method, this method supports Item Pagination . If Item Pagination is enabled, you must use this method when programmatically navigating through a table’s hierarchy. For more information on Item Pagination, see Support Item Pagination.

