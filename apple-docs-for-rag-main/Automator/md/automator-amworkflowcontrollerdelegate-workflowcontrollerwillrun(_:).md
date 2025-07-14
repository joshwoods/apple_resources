

- Automator
- AMWorkflowControllerDelegate
-  workflowControllerWillRun(\_:) 

Instance Method

# workflowControllerWillRun(\_:)

Notifies the delegate when the workflow controller object is about to run.

Mac Catalyst 14.0+macOS 10.4+

``` source
optional func workflowControllerWillRun(_ controller: AMWorkflowController)
```

## Parameters 

`controller`  

The workflow controller object to run.

## See Also

### Preparing to Run

func workflowController(AMWorkflowController, willRun: AMAction)

Notifies the delegate when the specified action is about to run.

