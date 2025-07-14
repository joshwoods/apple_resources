

- UIKit
- UITableViewDelegate
-  tableView(\_:canPerformPrimaryActionForRowAt:) 

Instance Method

# tableView(\_:canPerformPrimaryActionForRowAt:)

Asks the delegate whether to perform a primary action for the row at the specified index path.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    canPerformPrimaryActionForRowAt indexPath: IndexPath
) -> Bool
```

## Parameters 

`tableView`  

The table view object asking whether to perform a primary action.

`indexPath`  

The index path of the row.

## Return Value

true if the primary action can be performed; otherwise, false. If you don’t implement this method, the default return value is true when the table view isn’t in an editing state, and false when it is.

## Discussion

Primary actions allow you to distinguish between a distinct user action and a change in selection (like a focus change or other indirect selection change). A primary action occurs when a person selects a single row without extending an existing selection.

UIKit calls this method before tableView(_:performPrimaryActionForRowAt:).

## See Also

### Performing primary actions

func tableView(UITableView, performPrimaryActionForRowAt: IndexPath)

Tells the delegate to perform the primary action for the row at the specified index path.

