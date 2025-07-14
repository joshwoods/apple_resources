

- UIKit
- UIRefreshControl
-  beginRefreshing() 

Instance Method

# beginRefreshing()

Tells the control that a refresh operation was started programmatically.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func beginRefreshing()
```

## Discussion

Call this method when an external event source triggers a programmatic refresh of your scrolling view. In a table view, for example, if you use an instance of Timer to refresh the contents of the table view periodically, you would call this method as part of your timer handler. This method updates the state of the refresh control to reflect the in-progress refresh operation. When the refresh operation ends, be sure to call the endRefreshing() method to return the control to its default state.

## See Also

### Managing the refresh status

func endRefreshing()

Tells the control that a refresh operation has ended.

var isRefreshing: Bool

A Boolean value indicating whether a refresh operation has been triggered and is in progress.

