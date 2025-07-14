

- UIKit
- UITableViewDelegate
-  tableView(\_:didBeginMultipleSelectionInteractionAt:) 

Instance Method

# tableView(\_:didBeginMultipleSelectionInteractionAt:)

Tells the delegate when the user starts using a two-finger pan gesture to select multiple rows in a table view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    didBeginMultipleSelectionInteractionAt indexPath: IndexPath
)
```

## Parameters 

`tableView`  

The table view calling this method.

`indexPath`  

The index path of the item that the user touched to start the two-finger pan gesture.

## Discussion

Your implementation of this method is a good place to indicate, in the app’s user interface, that the user is selecting multiple rows; for example, you could replace an Edit or Select button with a Done button.

```
override func tableView(_ tableView: UITableView, didBeginMultipleSelectionInteractionAt indexPath: IndexPath) {
    // Replace the Edit button with Done, and put the
    // table view into editing mode.
    self.setEditing(true, animated: true)
}
```

## See Also

### Responding to row selections

Handling row selection in a table view

Detect when a user taps a table view cell so your app can take the next indicated action.

Selecting multiple items with a two-finger pan gesture

Accelerate user selection of multiple items using the multiselect gesture on table and collection views.

func tableView(UITableView, willSelectRowAt: IndexPath) -> IndexPath?

Tells the delegate a row is about to be selected.

func tableView(UITableView, didSelectRowAt: IndexPath)

Tells the delegate a row is selected.

func tableView(UITableView, willDeselectRowAt: IndexPath) -> IndexPath?

Tells the delegate that a specified row is about to be deselected.

func tableView(UITableView, didDeselectRowAt: IndexPath)

Tells the delegate that the specified row is now deselected.

func tableView(UITableView, shouldBeginMultipleSelectionInteractionAt: IndexPath) -> Bool

Asks the delegate whether the user can use a two-finger pan gesture to select multiple items in a table view.

func tableViewDidEndMultipleSelectionInteraction(UITableView)

Tells the delegate when the user stops using a two-finger pan gesture to select multiple rows in a table view.

