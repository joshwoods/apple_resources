

- UIKit
- UITableViewDelegate
-  indexPathForPreferredFocusedView(in:) 

Instance Method

# indexPathForPreferredFocusedView(in:)

Asks the delegate for the table view’s index path for the preferred focused view.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func indexPathForPreferredFocusedView(in tableView: UITableView) -> IndexPath?
```

## Parameters 

`tableView`  

A table view requesting the index path for preferred focus view.

## Return Value

An index path for the preferred focus row, or the default preferred focus view.

## Discussion

This functionality of this delegate method is equivalent to overriding UITableView class’s preferredFocusedView method in the UIFocusEnvironment protocol. If the UITableView class’s remembersLastFocusedIndexPath method is set to true, this method defines the index path that gets focused when the table view is focused for the first time.

The effects of this method may be ignored during or immediately after a view controller transition, such as a presentation dismissal or navigation stack pop. In such cases, the view controller attempts to restore focus to the item that was focused prior to the transition (for example, prior to the view controller being presented or pushed), which can take precedence over the effects of this method. To learn how to control or disable this behavior in the view controller, see restoresFocusAfterTransition.

## See Also

### Managing table view focus

func tableView(UITableView, canFocusRowAt: IndexPath) -> Bool

Asks the delegate whether the cell at the specified index path is itself focusable.

func tableView(UITableView, shouldUpdateFocusIn: UITableViewFocusUpdateContext) -> Bool

Asks the delegate whether the focus update specified by the context is allowed to occur.

func tableView(UITableView, didUpdateFocusIn: UITableViewFocusUpdateContext, with: UIFocusAnimationCoordinator)

Tells the delegate that a focus update specified by the context has just occurred.

func tableView(UITableView, selectionFollowsFocusForRowAt: IndexPath) -> Bool

Asks the delegate whether to relate selection and focus behavior for the row at the corresponding index path.

