

- UIKit
- UITableViewDelegate
-  tableView(\_:selectionFollowsFocusForRowAt:) 

Instance Method

# tableView(\_:selectionFollowsFocusForRowAt:)

Asks the delegate whether to relate selection and focus behavior for the row at the corresponding index path.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    selectionFollowsFocusForRowAt indexPath: IndexPath
) -> Bool
```

## Parameters 

`tableView`  

The table view making the request.

`indexPath`  

The index path of the row to determine selection behavior for.

## Return Value

true if you want to automatically select the row at the specified index path when focus moves to it; otherwise, false.

## Discussion

If the table view’s selectionFollowsFocus property is true and you return false from this delegate method, focus still moves to the row when the user selects it. However, when focus moves to the row, the row doesn’t automatically select.

## See Also

### Managing table view focus

func tableView(UITableView, canFocusRowAt: IndexPath) -> Bool

Asks the delegate whether the cell at the specified index path is itself focusable.

func tableView(UITableView, shouldUpdateFocusIn: UITableViewFocusUpdateContext) -> Bool

Asks the delegate whether the focus update specified by the context is allowed to occur.

func tableView(UITableView, didUpdateFocusIn: UITableViewFocusUpdateContext, with: UIFocusAnimationCoordinator)

Tells the delegate that a focus update specified by the context has just occurred.

func indexPathForPreferredFocusedView(in: UITableView) -> IndexPath?

Asks the delegate for the table view’s index path for the preferred focused view.

