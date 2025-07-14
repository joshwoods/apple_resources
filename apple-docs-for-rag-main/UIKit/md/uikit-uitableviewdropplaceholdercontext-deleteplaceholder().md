

- UIKit
- UITableViewDropPlaceholderContext
-  deletePlaceholder() 

Instance Method

# deletePlaceholder()

Removes an unneeded placeholder cell from the table view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func deletePlaceholder() -> Bool
```

**Required**

## Return Value

true if the placeholder cell was removed, or false if the cell was no longer in the table view.

## Discussion

Call this method on your app’s main thread to remove a placeholder cell without swapping in a new cell. You might call this method if the user chooses to undo the insertion of a cell or if the contents of the table view changed.

