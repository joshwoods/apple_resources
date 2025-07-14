

- UIKit
- UIRefreshControl
-  isRefreshing 

Instance Property

# isRefreshing

A Boolean value indicating whether a refresh operation has been triggered and is in progress.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var isRefreshing: Bool { get }
```

## See Also

### Managing the refresh status

func beginRefreshing()

Tells the control that a refresh operation was started programmatically.

func endRefreshing()

Tells the control that a refresh operation has ended.

