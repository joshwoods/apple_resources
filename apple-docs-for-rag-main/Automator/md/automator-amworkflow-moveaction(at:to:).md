

- Automator
- AMWorkflow
-  moveAction(at:to:) 

Instance Method

# moveAction(at:to:)

Moves the action from the specified start position to the specified end position in the receiving workflow.

Mac Catalyst 14.0+macOS 10.4+

``` source
func moveAction(
    at startIndex: Int,
    to endIndex: Int
)
```

## Parameters 

`startIndex`  

The start position of the action to move.

`endIndex`  

The end position for the action that is moved.

## Discussion

If either index is invalid, this method does nothing.

## See Also

### Manipulating the Workflow’s Actions

func addAction(AMAction)

Adds the specified action at the end of the receiving workflow.

func insertAction(AMAction, at: Int)

Inserts the specified action at the specified position of the receiving workflow.

func removeAction(AMAction)

Removes the specified action from the workflow.

