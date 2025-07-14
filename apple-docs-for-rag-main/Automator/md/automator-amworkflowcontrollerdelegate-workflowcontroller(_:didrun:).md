

- Automator
- AMWorkflowControllerDelegate
-  workflowController(\_:didRun:) 

Instance Method

# workflowController(\_:didRun:)

Notifies the delegate when the specified action finishes running.

Mac Catalyst 14.0+macOS 10.4+

``` source
optional func workflowController(
    _ controller: AMWorkflowController,
    didRun action: AMAction
)
```

## Parameters 

`controller`  

The controller object sending the message.

`action`  

The workflow action that ran.

## See Also

### Running

func workflowControllerDidRun(AMWorkflowController)

Notifies the delegate when the workflow controller object finishes running.

