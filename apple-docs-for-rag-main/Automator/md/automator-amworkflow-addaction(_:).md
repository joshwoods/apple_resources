

- Automator
- AMWorkflow
-  addAction(\_:) 

Instance Method

# addAction(\_:)

Adds the specified action at the end of the receiving workflow.

Mac Catalyst 14.0+macOS 10.4+

``` source
func addAction(_ action: AMAction)
```

## Parameters 

`action`  

The action to add.

## Discussion

The workflow retains the action but does not copy it.

## See Also

### Manipulating the Workflow’s Actions

func insertAction(AMAction, at: Int)

Inserts the specified action at the specified position of the receiving workflow.

func moveAction(at: Int, to: Int)

Moves the action from the specified start position to the specified end position in the receiving workflow.

func removeAction(AMAction)

Removes the specified action from the workflow.

