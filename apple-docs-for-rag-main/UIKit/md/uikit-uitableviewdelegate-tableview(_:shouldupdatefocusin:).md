

- UIKit
- UITableViewDelegate
-  tableView(\_:shouldUpdateFocusIn:) 

Instance Method

# tableView(\_:shouldUpdateFocusIn:)

Asks the delegate whether the focus update specified by the context is allowed to occur.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    shouldUpdateFocusIn context: UITableViewFocusUpdateContext
) -> Bool
```

## Parameters 

`tableView`  

A table view in which the focus update is occurring.

`context`  

An instance of UIFocusUpdateContext class, contains metadata for the focus related update.

## Return Value

true if the focus should update; otherwise false.

## Discussion

The functionality of this delegate method is equivalent to overriding UITableView class’s shouldUpdateFocus(in:) method. This delegate method provides additional UITableView-related information in its context parameter, such as the index paths for the previously and next focused views. Note that, these index paths are only available if their views are contained within the table view. To learn more about the information provided by the context, see UITableViewFocusUpdateContext.

## See Also

### Managing table view focus

func tableView(UITableView, canFocusRowAt: IndexPath) -> Bool

Asks the delegate whether the cell at the specified index path is itself focusable.

func tableView(UITableView, didUpdateFocusIn: UITableViewFocusUpdateContext, with: UIFocusAnimationCoordinator)

Tells the delegate that a focus update specified by the context has just occurred.

func indexPathForPreferredFocusedView(in: UITableView) -> IndexPath?

Asks the delegate for the table view’s index path for the preferred focused view.

func tableView(UITableView, selectionFollowsFocusForRowAt: IndexPath) -> Bool

Asks the delegate whether to relate selection and focus behavior for the row at the corresponding index path.

