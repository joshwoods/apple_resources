

- AppKit
- NSMatrix
-  doubleAction 

Instance Property

# doubleAction

The action sent to the target of the receiver when the user double-clicks a cell.

macOS

``` source
@MainActor
var doubleAction: Selector? { get set }
```

## Discussion

The double-click action of an NSMatrix is sent after the appropriate single-click action (for the NSCell clicked, or for the NSMatrix if the NSCell doesn’t have its own action). If there is no double-click action and the NSMatrix doesn’t ignore multiple clicks, the single-click action is sent twice. If the value of this property is a non-`nil` selector, this property also sets `ignoresMultiClick` to false; otherwise, it leaves `ignoresMultiClick` unchanged.

## See Also

### Related Documentation

var action: Selector?

The default action-message selector associated with the control.

var ignoresMultiClick: Bool

A Boolean value indicating whether the receiver ignores multiple clicks made in rapid succession.

var target: AnyObject?

The target object that receives action messages from the cell.

### Managing and Sending Action Messages

func sendAction() -> Bool

If the selected cell has both an action and a target, sends its action to its target.

func sendAction(Selector, to: Any, forAllCells: Bool)

Iterates through the cells in the receiver, sending the specified selector to an object for each cell.

func sendDoubleAction()

Sends the double-click action message to the target of the receiver.

