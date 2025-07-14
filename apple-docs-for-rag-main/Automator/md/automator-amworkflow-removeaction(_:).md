

- Automator
- AMWorkflow
-  removeAction(\_:) 

Instance Method

# removeAction(\_:)

Removes the specified action from the workflow.

Mac Catalyst 14.0+macOS 10.4+

``` source
func removeAction(_ action: AMAction)
```

## Parameters 

`action`  

The action to be removed.

## Discussion

The action receives an `AMAction closed` message before being released.

## See Also

### Manipulating the Workflow’s Actions

func addAction(AMAction)

Adds the specified action at the end of the receiving workflow.

func insertAction(AMAction, at: Int)

Inserts the specified action at the specified position of the receiving workflow.

func moveAction(at: Int, to: Int)

Moves the action from the specified start position to the specified end position in the receiving workflow.

