

- UIKit
- UITableViewDelegate
-  tableView(\_:canFocusRowAt:) 

Instance Method

# tableView(\_:canFocusRowAt:)

Asks the delegate whether the cell at the specified index path is itself focusable.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    canFocusRowAt indexPath: IndexPath
) -> Bool
```

## Parameters 

`tableView`  

The table view requesting this information.

`indexPath`  

An index path locating a row in `tableView`.

## Return Value

true if the row indicated by `indexPath`; otherwise, false.

## Discussion

The functionality of this delegate method is equivalent to overriding the cell’s canBecomeFocused method. If true is returned, then the cell at the specified index path is focusable, meaning none of its contents can be focused. Returningfalse means the cell itself is not focusable, however this does not prevent any of its contents from being focused. If this method is not implemented, then the return value is assumed to be true.

## See Also

### Managing table view focus

func tableView(UITableView, shouldUpdateFocusIn: UITableViewFocusUpdateContext) -> Bool

Asks the delegate whether the focus update specified by the context is allowed to occur.

func tableView(UITableView, didUpdateFocusIn: UITableViewFocusUpdateContext, with: UIFocusAnimationCoordinator)

Tells the delegate that a focus update specified by the context has just occurred.

func indexPathForPreferredFocusedView(in: UITableView) -> IndexPath?

Asks the delegate for the table view’s index path for the preferred focused view.

func tableView(UITableView, selectionFollowsFocusForRowAt: IndexPath) -> Bool

Asks the delegate whether to relate selection and focus behavior for the row at the corresponding index path.

