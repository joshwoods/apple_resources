

- AppKit
- NSMatrix
-  sendAction() 

Instance Method

# sendAction()

If the selected cell has both an action and a target, sends its action to its target.

macOS

``` source
@MainActor
func sendAction() -> Bool
```

## Return Value

true if an action was successfully sent to a target. If the selected cell is disabled, this method does nothing and returns false.

## Discussion

If the cell has an action but no target, its action is sent to the target of the receiver. If the cell doesn’t have an action, or if there is no selected cell, the receiver sends its own action to its target.

## See Also

### Related Documentation

var action: Selector?

The action performed by the cell.

var target: AnyObject?

The object that receives the cell’s action messages.

### Managing and Sending Action Messages

func sendAction(Selector, to: Any, forAllCells: Bool)

Iterates through the cells in the receiver, sending the specified selector to an object for each cell.

var doubleAction: Selector?

The action sent to the target of the receiver when the user double-clicks a cell.

func sendDoubleAction()

Sends the double-click action message to the target of the receiver.

