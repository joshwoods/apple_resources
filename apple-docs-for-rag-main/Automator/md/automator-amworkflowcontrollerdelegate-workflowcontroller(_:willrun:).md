

- Automator
- AMWorkflowControllerDelegate
-  workflowController(\_:willRun:) 

Instance Method

# workflowController(\_:willRun:)

Notifies the delegate when the specified action is about to run.

Mac Catalyst 14.0+macOS 10.4+

``` source
optional func workflowController(
    _ controller: AMWorkflowController,
    willRun action: AMAction
)
```

## Parameters 

`controller`  

The controller object sending the message.

`action`  

The workflow action to run.

## See Also

### Preparing to Run

func workflowControllerWillRun(AMWorkflowController)

Notifies the delegate when the workflow controller object is about to run.

