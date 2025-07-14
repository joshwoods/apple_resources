

- Automator
- AMWorkflow
-  insertAction(\_:at:) 

Instance Method

# insertAction(\_:at:)

Inserts the specified action at the specified position of the receiving workflow.

Mac Catalyst 14.0+macOS 10.4+

``` source
func insertAction(
    _ action: AMAction,
    at index: Int
)
```

## Parameters 

`action`  

The action to insert.

`index`  

The position in the receiver at which to insert the action. If the position is invalid, this method does nothing.

## Discussion

The workflow retains the action but does not copy it.

## See Also

### Manipulating the Workflow’s Actions

func addAction(AMAction)

Adds the specified action at the end of the receiving workflow.

func moveAction(at: Int, to: Int)

Moves the action from the specified start position to the specified end position in the receiving workflow.

func removeAction(AMAction)

Removes the specified action from the workflow.

